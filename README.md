# Choocide
An Ada-coded Train signaling system


To DO:
  Train State:- Stopped, Moving, Siding
  Data Attributes of Train:- Train Number, Speed, Direction(UP/DOWN), Signal status

Track Layout:-
    GOING TO RIGHT IS UP
    GOING TO LEFT IS DOWN

Main Line  (EnterUP---->)==========Sig1(Up)===========================Sig2(Down)===============(<-----Enter Down)
Siding                                   ^==============================^


Req:-
      *System should not give two trains a green on main
      *If there is a train in the siding, switch locked to Main only
      *Impose a track speed limit, if exceeded, show red
      *If a train stops on the main, automatically divert incoming trains to halt in siding till tracks are cleared
      *assign priority to trains, and give signals according to the same(passeners>frieghts)
      *Always give siding switch to lower priority train
      *If a train halts halfway through the siding, red signal the entire main (2 track sections on each side of the section of concern)
      *If a train passes multiple Reds(2), divert to the siding to allow it to derail (freight only)
      

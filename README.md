graph LR
    %% Define actors with simple stick figures
    Doctor(["○<br/>┃<br/>╱╿╲"])
    User(["○<br/>┃<br/>╱╿╲"])

    %% Label actors
    Doctor --- |Administrator|Doctor
    User --- |Regular User|User
    
    %% Use cases in oval shapes arranged vertically in the middle
    Register((Register))
    Login((Login))
    Upload((Upload Fracture Image))
    Detect((View Detection Result))
    Report((Generate Report))
    Chat((Access ChatBot))
    History((View History))
    Logout((Logout))

    %% Connect actors to use cases horizontally
    Doctor --- Register --- User
    Doctor --- Login --- User
    Doctor --- Upload --- User
    Doctor --- Detect --- User
    Doctor --- Report --- User
    Doctor --- Chat --- User
    Doctor --- History --- User
    Doctor --- Logout --- User

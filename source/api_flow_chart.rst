API Flow Chart
==================
.. tip::
    Login is required to control the laser power.


.. mermaid::

    flowchart TD;
        classDef yellow fill:yellow

        Start[Start] -->Discover[Discover]
        Discover --> |SerialNumber / IP| Connect[Connect]
        Connect--> Login[Login]:::yellow
        Login --> |Mode Selection| Mode{SetOutputMode}
        Mode --> |2D| 2D[2D Mode]
        Mode --> |3D| 3D[3D Mode]
        2D --> CalculateTransformMatrixFromChessPattern[CalculateTransformMatrixFromChessPattern]
        2D --> Capture2D[Capture2D]
        3D --> Capture3D[Capture3D]
        CalculateTransformMatrixFromChessPattern --> Disconnect[Disconnect]
        Capture2D --> Disconnect[Disconnect]
        Capture3D --> Disconnect[Disconnect]
        Disconnect[Disconnect] --> End[End]



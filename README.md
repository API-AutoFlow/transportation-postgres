# transportation-postgres
Summary

    This is a use case for transportation system.
    Postgres is used to manage database. 

    - First Video Demo for Developers:
        https://www.youtube.com/embed/kyrjl85Oo6Q
        in this video, I introduced our problem and the fundamentals of the solution.
        And created two first features: (1)get-buses (2)insert-bus
        then I used some basic actions:
            - JSON / Decode
            - String / Join
            - Postgres / Query
        
    - Second Video Demo for Developers:
        https://www.youtube.com/watch?v=ZTPNEC3iTRQ
        using new actions: 
            - Iteration / For-Each 
            - Array / Insert-at 
            - Array / Sort 
            - Data / Set 

        Also, to do similar actions in API AutoFlow, we used " Copy / Paste ".
        
     - Third Video Demo for Developers:
        https://youtu.be/CRXFtCQYdGo
        in this video we presented:
            - Timers
            - Files
            - Flows
            - integration with Slack Webhook
 
            
      - New features after "Third Video":
            - EndPoint: /insert-bus-route : to insert/update bus route
                request-body: bus_id & station_id[]
            - EndPoint: /update-timers : turns timers on/off
                request-body: {"update":"on/off","check":"on/off","clean":"on/off"}
                                "update" = "update bus position"        timer
                                "check"  = "check bus situation"        timer
                                "clean"  = "clean bus_position table"   timer
            - EndPoint: /simulate-position: this is a GET method to resieve different positions for bus_1
                                            every GET request recieves different Lat&Long

 Hi, I’m @AndreaTodeschi, a 26 years Italian web dev
At the start of 2021 I made a resolution to finish what I had started learning in university a couple years earlier, coding.

I picked up Java and SQL, using PostgreSQL, Hibernate and JavaFX to try and build a personal idea I have since a long time. I managed to get it working on the base functionality, but I have since decided to rebuild the entire project with node and react to make it more easily manageable.

I started learning web development, HTML, CSS and JavaScript (along with a little bit of Python and Django) and build a frontend with Reactjs (well it's completely in TypeScript since not having type checking really bothered me).

I now released my little project to production and I monetized it, https://reusegm.com.
It uses NextJS for the main website and customer panel frontend, Auth0 for customer authentication, meanwhile the business app is made in React, as load times are a non issue.
The backend is managed with Dokku, with a server with an Express API and also a GraphQL endpoint using Apollo Express. I manage database entities with TypeORM and GraphQL with type-graphql as I feel they mesh together really well making it easy to manage both at the same time in a clean way.
I have built a little statistics page, the data is fetched from a separate docker container, which has a waitress local server in my backend who accepts the requests, fetches the data and uses Pandas to transform it before sending it back to the node backend which in turns serves it to the client.
While I could have just called the scripts to fetch the data directly from node, I felt it was going to be nice experimenting with docker networks and try out the microservices architecture, which I'll probably end up implementing more broadly going forward as I feel it's easier to manage the bigger the project gets.

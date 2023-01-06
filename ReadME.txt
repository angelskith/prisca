creating dynamic file/path equivalent to wild card => [project].js - this file could take any name or parameter
    - import {useRouter} from 'next/router' to inject the dynamic file to your component
    - used as const router = useRouter()
    - router.query => to get the value inserted on the path url
        - using 'query' you can send a request to some backend server.
        - fetching the piece of data with an id of *router.query.projectid
    - you can also create a dynamic folder with dynamic file where both folder and file could accept a value from path url
    - you can also used the dynamic folder & file as an object value using router.query

create like a spread operator [...fileName] to catch all path *host/any/any/aany (array)

Mapping => clients.map((client) => (
    <li key={client.id}>
        <Link href={`/clients/${client.id}`}>{client.name}</Link>
    </li>
))

router.push() - work same as <Link> programmatically

-------- REACT
for reusable components pass the data through props
    - Create a seperate component with dynamic data then change it or declare it on main component (*import the dynamic components)
for built-in components(undeclared/uncalled in any function) point the props to forward the function where it will be received.
    - https://www.udemy.com/course/nextjs-react-the-complete-guide/learn/lecture/25146622#questions

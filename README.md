# Booyah entry task

--------

## 1. Feature requirement
### Feature
1. Implement a basic user manager system, allow users to log in and register;
2. After a user log in, he/she can query his/her own information;
3. After a user log in, he/she can edit his/her information, like: profile picture, nickname, etc;

### Domain
User information includes: 
1. Username (cannot be changed)
2. Nickname
3. Profile picture

For test purpose, the initial user data can be directly insert into database. 
Make sure there are at least 10 million user accounts in the test database.

## 2. Technical requirement
### Design Constraint
1. Separate HTTP server and TCP server, and put the main logic on TCP server;
2. Backend authentication logic should be done in the TCP server;
3. User information must be stored in a MySQL database;
4. Use standard library whenever possible;
6. For each HTTP request, web interface will send a TCP request to the TCP server, which will handle business logic and query the database;

### Design Considerations
- Performance
- Robustness
- Security

### Time Limit
You need to finish this task in 5 working days.

### Performance
- Supports up to 1000 login requests per second (from at least 200 unique users)
- Supports up to 1000 concurrent http requests

### Environment
- Server: Virtual Machine on Working PC
- OS: CentOS 7 x64 or Ubuntu 14.04 above
- DB: MySQL 5.5 or above
- Client: Chrome and Firefox

## 3. Deliverables
1. Project source
2. Design document
3. Installation and maintenance documentation 
4. Performance tests report
5. Concluding report

## 4. References
1. Go: http://golang.org
2. Coding style: https://github.com/golang/go/wiki/CodeReviewComments
3. Test suite: https://golang.org/pkg/testing/
4. Profiling: http://blog.golang.org/profiling-go-programs
5. Go MySQL client: https://github.com/go-sql-driver/mysql
6. Go Redis Client: https://github.com/go-redis/redis
7. Go Web application example: https://golang.org/doc/articles/wiki/

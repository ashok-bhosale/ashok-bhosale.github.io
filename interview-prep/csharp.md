# C# / .NET Interview Questions — Distinct & Categorized

> Consolidated from the uploaded **C Sharp Basic & Advanced.md** source. Repeated questions have been consolidated so each distinct question appears once.

## Overview

- **Original question entries:** 1,950
- **Repeated/near-identical entries consolidated:** 320
- **Distinct questions retained:** **1,630**
- **Categories:** **20**
- **Organization:** beginner → advanced C# → .NET → web/API → data → architecture → cloud/security → system design.

## Table of Contents

1. [C# Fundamentals & Language Basics](#c#-fundamentals-and-language-basics)
2. [Types, Variables, Operators & Control Flow](#types-variables-operators-and-control-flow)
3. [Object-Oriented Programming](#object-oriented-programming)
4. [Collections, Iterators & Generics](#collections-iterators-and-generics)
5. [Delegates, Events, Lambdas & Functional C#](#delegates-events-lambdas-and-functional-c#)
6. [LINQ & Expression Trees](#linq-and-expression-trees)
7. [Exception Handling & Error Management](#exception-handling-and-error-management)
8. [Async, Multithreading & Concurrency](#async-multithreading-and-concurrency)
9. [Memory Management, GC & Resource Management](#memory-management-gc-and-resource-management)
10. [.NET Runtime, CLR & Advanced C# Internals](#net-runtime-clr-and-advanced-c#-internals)
11. [Reflection, Attributes, Serialization & I/O](#reflection-attributes-serialization-and-i/o)
12. [Dependency Injection & Application Infrastructure](#dependency-injection-and-application-infrastructure)
13. [ASP.NET Core, Web API & Communication](#aspnet-core-web-api-and-communication)
14. [Entity Framework Core & Data Access](#entity-framework-core-and-data-access)
15. [Design Patterns, SOLID & Clean Architecture](#design-patterns-solid-and-clean-architecture)
16. [DDD, Microservices, Messaging & Distributed Systems](#ddd-microservices-messaging-and-distributed-systems)
17. [Docker, Kubernetes, DevOps & Observability](#docker-kubernetes-devops-and-observability)
18. [Cloud Architecture, Security & Reliability](#cloud-architecture-security-and-reliability)
19. [System Design & Performance Engineering](#system-design-and-performance-engineering)
20. [Testing, Leadership & Architecture Governance](#testing-leadership-and-architecture-governance)

## Deduplication Note

- Exact repeats and near-identical wording such as `What is X?`, `X?`, and equivalent `What is a X?` forms were consolidated.
- Questions with a different scope or deeper architectural focus were retained as separate questions.
- The wording and terminology are based on the uploaded source; this file reorganizes rather than replaces the source material.

## 1. C# Fundamentals & Language Basics

**324 distinct questions**

1. What is C#?
2. What are the features of C#?
3. What is the CLR?
4. What is CTS?
5. What is CLS?
6. What is MSIL/IL?
7. What is the .NET runtime?
8. What are namespaces?
9. What is the Main() method?
10. Difference between .NET Framework and .NET?
11. What are assemblies?
12. What are manifests?
13. What are references?
14. What is the Global Assembly Cache (GAC)?
15. What is JIT compilation?
16. Types of JIT compiler?
17. What are value types?
18. What are reference types?
19. Difference between stack and heap?
20. What is boxing?
21. What is unboxing?
22. What are identifiers?
23. What are keywords?
24. What are literals?
25. What are comments in C#?
26. What is implicit vs explicit conversion?
27. What is the difference between == and Equals()?
28. What is switch statement?
29. What is a method?
30. Difference between overloading and overriding?
31. What are optional parameters?
32. Named parameters?
33. ref keyword?
34. out keyword?
35. in keyword?
36. params keyword?
37. Recursive methods?
38. Static methods?
39. Expression-bodied methods?
40. Tuples?
41. Global Using?
42. What is top-level statements?
43. Required properties?
44. Ahead-of-Time Compilation?
45. Performance optimization?
46. High-performance C# coding practices?
47. High-performance coding practices?
48. What is ReaderWriterLockSlim?
49. What is secrets management?
50. What are the main features of C#?
51. What is the .NET Framework?
52. What is the difference between JIT and AOT?
53. What is the difference between C# and .NET?
54. What is a namespace?
55. What is an assembly?
56. What is the difference between exe and dll?
57. Difference between stack and heap memory?
58. What are nullable types?
59. What is a struct?
60. Difference between struct and class?
61. What is an enum?
62. What is a constructor?
63. Types of constructors in C#?
64. What is a static constructor?
65. What is a destructor?
66. What is the “using” keyword?
67. What is type inference?
68. What is `var` vs `dynamic`?
69. What is the difference between const and readonly?
70. What is .NET Core?
71. Differences between .NET Framework and .NET Core?
72. What is cross-platform?
73. What is appsettings.json?
74. What are hosted services?
75. What is IHostedService?
76. What is BackgroundService?
77. What is GCSettings?
78. What is trimming?
79. What are global usings?
80. What is implicit namespaces?
81. What is .NET?
82. What is managed code?
83. What is unmanaged code?
84. What is JIT compiler?
85. What is MSIL?
86. What is namespace?
87. What is type casting?
88. What is var keyword?
89. What is dynamic keyword?
90. What is default value?
91. What are constants?
92. What is readonly?
93. What are operators in C#?
94. What is ternary operator?
95. What is string interpolation?
96. What is escape sequence?
97. What is parsing?
98. What is TryParse?
99. What is Main method?
100. What are command-line arguments?
101. What is checked vs unchecked?
102. What is enum?
103. What is struct?
104. What is class?
105. What is object?
106. What is method?
107. What is parameter vs argument?
108. What is return type?
109. What is recursion?
110. What is loop?
111. Difference between for and foreach?
112. What is break?
113. What is continue?
114. What is goto?
115. What is metadata?
116. What is Web API?
117. What is validation?
118. What is session?
119. What is state management?
120. What is NLog?
121. What is configuration?
122. What is environment?
123. What is retry pattern?
124. What is bulkhead?
125. What is layered architecture?
126. What is Moq?
127. What is xUnit?
128. What is NUnit?
129. What is Git?
130. What is version control?
131. What is branching?
132. What is merging?
133. What is code review?
134. What is static analysis?
135. What is SonarQube?
136. What is security best practices?
137. What is hashing?
138. What is SSL/TLS?
139. What is load balancing?
140. What is telemetry?
141. What is health check?
142. What is feature toggle?
143. What is rollback?
144. What is high availability?
145. What is fault tolerance?
146. What is SLA?
147. What is SLO?
148. What is SLA vs SLO?
149. What is documentation?
150. What is API documentation?
151. What is code quality?
152. What is refactoring?
153. What is maintainability?
154. What is readability?
155. What is best practice in C#?
156. What are the main features of C# 12/11/10?
157. What is the difference between ref and out keywords?
158. Explain value types vs reference types.
159. What is boxing and unboxing?
160. What is the difference between dynamic and var?
161. What is a struct? When should you use it?
162. What is using statement in C#?
163. What is GC?
164. .NET Core: What is it?
165. Difference between .NET Framework and .NET Core?
166. What is cross-platform support in .NET Core?
167. What is Main() method in .NET Core?
168. What is ConfigureServices() method?
169. What is Configure() method?
170. Explain IApplicationBuilder.
171. What is HostBuilder?
172. How configuration works in .NET Core?
173. What are configuration providers?
174. What are Options pattern?
175. How to register services in DI?
176. How does .NET Core logging work?
177. What is ILogger?
178. What are background worker services?
179. What is ViewModel?
180. What is ViewBag, ViewData, TempData?
181. What is Razor View Engine?
182. What are TagHelpers?
183. What are ViewComponents?
184. Difference between Partial View and ViewComponent?
185. What is AntiForgeryToken?
186. How validation works?
187. What is Data Annotation?
188. What is ModelState?
189. What are Areas?
190. What is Layout page?
191. How to cache views?
192. How does session work in .NET Core?
193. How to return problem details (RFC 7807) from APIs?
194. How to validate input models and return errors consistently?
195. Recommended status codes for create/update/delete/not found?
196. What is content negotiation and how is it implemented?
197. Support both JSON and XML in Web API?
198. File uploads and large file streaming in Web API?
199. Conditional requests with ETags/If-Modified-Since?
200. Design APIs to be backward compatible?
201. What is ProblemDetails and how to extend it?
202. Handle long-running jobs (202 Accepted + polling, webhooks)?
203. Implement file downloads and range requests?
204. Secure admin-only endpoints with policies?
205. Expose health checks for APIs?
206. Return hypermedia links (HATEOAS)?
207. Structure RESTful URL hierarchy for nested resources?
208. Deprecate API endpoints gracefully?
209. Protect against over-posting / mass assignment?
210. Request/response compression?
211. Explain statelessness and its impact on scaling.
212. Resource vs representation in REST?
213. When to use PUT vs PATCH?
214. Idempotent methods and which verbs are idempotent?
215. 200 vs 201 vs 204 vs 202—when?
216. Difference between 4xx and 5xx families?
217. Design consistent error payloads across services?
218. What is HATEOAS and current relevance?
219. Handle breaking changes in APIs?
220. What is an API contract and how to enforce it?
221. Design rate limits per consumer tiers?
222. Design multi-tenant APIs (headers, tokens, domains)?
223. Handle partial failures in composite endpoints?
224. Richardson Maturity Model for REST?
225. Model long-running operations (202 + retry-after + status)?
226. Manage API lifecycle (design, publish, deprecate, retire)?
227. Scopes vs claims—differences?
228. Rotate signing keys—how?
229. Refresh tokens—how to handle securely?
230. What is PKCE and when needed?
231. Client credentials flow for M2M APIs?
232. What is mTLS and when to use it?
233. Detect/mitigate brute-force / credential stuffing?
234. Customize operation IDs, schema names, and tags?
235. NSwag vs Swashbuckle—tradeoffs?
236. Define service boundaries (business capability vs data-driven)?
237. Detect and resolve circular dependencies between services?
238. Idempotent REST endpoints for POST—how?
239. Strategies for distributed locking?
240. Propagate correlation IDs across services?
241. Retries + deduplication in consumers?
242. Bulkhead isolation between services?
243. Data ownership and enforcement across services?
244. Combine multiple policies (PolicyWrap)?
245. What is hedging and when to use it?
246. Design time-outs at each layer?
247. Cache-aside vs write-through vs write-behind?
248. Redis keys and eviction policies?
249. Per user/tenant caching with proper scoping?
250. Cache HTTP responses in ASP.NET Core?
251. Avoid thundering herd (request coalescing)?
252. Handle stale data vs consistency (TTL, refresh-ahead)?
253. Implement request batching for performance?
254. Token bucket vs leaky bucket algorithm?
255. Handle 429 Too Many Requests programmatically?
256. Optimize Include graphs and avoid cartesian explosions?
257. Split vs Single query for Include—when?
258. Model many-to-many relationships and join control?
259. AsSplitQuery vs AsSingleQuery performance impact?
260. Database-agnostic EF models (provider-specific annotations)?
261. Seeding strategies for tenants/environments?
262. Secure connection strings and rotate them?
263. Log generated SQL safely in production?
264. Difference between ACID and BASE properties?
265. Design idempotent consumers with message stores?
266. Design poison message handling?
267. Test end-to-end data flows (producer  broker  consumer)?
268. Ensure idempotent writes to the database from consumers?
269. ENTRYPOINT vs CMD?
270. Deterministic builds with pinned base images?
271. Alpine-based images—when to use?
272. Bind mounts vs volumes?
273. What is kubelet?
274. What are Pods?
275. ClusterIP vs NodePort vs LoadBalancer?
276. How do Secrets work?
277. Mount volumes in Pods?
278. Readiness vs liveness probes?
279. Scale Pods automatically (HPA)?
280. Perform rolling updates?
281. Isolate namespaces?
282. What is a network policy?
283. Tolerations and taints?
284. Debug failing Pods (logs, exec, describe)?
285. Instrument .NET APIs for tracing?
286. What are spans and traces?
287. What is W3C Trace Context?
288. Export traces from .NET to Jaeger/Zipkin/App Insights?
289. Structured logging and importance?
290. Console logging vs structured JSON logging?
291. Log enrichment and correlation?
292. Avoid logging sensitive data?
293. What is log sampling?
294. Choose log retention policies?
295. Difference between metrics, logs, and traces?
296. What is RED method?
297. What is USE method?
298. Set up health checks in ASP.NET Core?
299. Liveness vs readiness health checks?
300. Add custom health checks (DB, cache, broker)?
301. Tools for .NET performance (dotTrace, PerfView, dotMemory)?
302. Troubleshoot CPU spikes?
303. Capture custom application metrics?
304. Domain entities vs aggregates?
305. Difference between queries and commands?
306. Configure autoscaling rules?
307. What is Infrastructure-as-Code (IaC)?
308. What is a replay attack and how to stop it?
309. Enforce HTTPS in .NET?
310. Protect connection strings and secrets in production?
311. What is secure coding?
312. AuthN vs AuthZ?
313. Detect token tampering?
314. Implement row-level security?
315. How does the .NET Garbage Collector work?
316. What is Span and how it reduces allocations?
317. What is Memory in .NET?
318. What is boxing allocation and avoiding it?
319. What is PGO (Profile Guided Optimization)?
320. What is a Completion Port?
321. Bounded vs unbounded channel?
322. What is a background worker service?
323. Immutable data structures and why use them?
324. Scale Web API to handle 100K+ requests/min?

## 2. Types, Variables, Operators & Control Flow

**35 distinct questions**

1. What are variables?
2. Difference between var, dynamic, and object?
3. What are primitive data types?
4. What is type conversion?
5. What is Parse()?
6. What is TryParse()?
7. What is Convert class?
8. What is nullable type?
9. What is Nullable<T>?
10. What is default value of types?
11. What is sizeof operator?
12. What is typeof operator?
13. What is GetType()?
14. What is dynamic typing?
15. Types of operators in C#
16. What is ReferenceEquals()?
17. What is null-coalescing operator ??
18. What is null-conditional operator ?.
19. What is pattern matching?
20. What is is operator?
21. What is as operator?
22. Difference between ++i and i++?
23. if statement
24. Switch Expressions?
25. while loop
26. do-while loop
27. for loop
28. foreach loop
29. break statement
30. continue statement
31. goto statement
32. What is nullable reference types?
33. Pattern Matching evolution?
34. What is a nullable type?
35. Core constraints of REST?

## 3. Object-Oriented Programming

**122 distinct questions**

1. What is operator overloading?
2. What is method overloading?
3. What is method overriding?
4. What are extension methods?
5. What is OOP?
6. What are OOP principles?
7. What is encapsulation?
8. What is abstraction?
9. What is inheritance?
10. What is polymorphism?
11. What is a class?
12. What is an object?
13. What is constructor?
14. What is destructor?
15. Types of constructors?
16. Copy constructor?
17. What is static constructor?
18. Private constructor?
19. What is `this` keyword?
20. What is `base` keyword?
21. What are access modifiers?
22. Public vs private?
23. Protected vs internal?
24. What is sealed class?
25. What is abstract class?
26. What is interface?
27. Multiple inheritance in C#?
28. Virtual methods?
29. What is override keyword?
30. Difference between abstract class and interface?
31. What is explicit interface implementation?
32. Default interface methods?
33. What are partial classes?
34. Nested classes?
35. Static classes?
36. Object initializers?
37. Collection initializers?
38. Record types?
39. Init-only properties?
40. Immutable objects?
41. Struct vs class?
42. Readonly struct?
43. Primary constructors?
44. What is singleton pattern?
45. Records?
46. Records internals?
47. Init-only setters?
48. Switch expressions internals?
49. Dynamic keyword internals?
50. What is virtual keyword?
51. What is an abstract class?
52. What is an interface?
53. Differences between abstract class and interface?
54. Can interfaces contain fields?
55. Can interfaces have default implementations?
56. What is multiple inheritance?
57. Does C# support multiple inheritance?
58. What is tightly coupled vs loosely coupled?
59. What is composition?
60. What is aggregation?
61. What are sealed methods?
62. What are indexers?
63. What are properties?
64. Auto-implemented properties?
65. What is encapsulation in C#?
66. What is a multicast delegate?
67. What is an event?
68. Difference between event and delegate?
69. What is a lambda expression?
70. What is anonymous method?
71. Can you overload every operator?
72. What is shadowing vs overriding?
73. What is record type?
74. Difference between interface and abstract class?
75. How does C# support it?
76. What is default constructor?
77. What is parameterized constructor?
78. What is constructor chaining?
79. What is access modifier?
80. Types of access modifiers?
81. What is private?
82. What is public?
83. What is protected?
84. What is internal?
85. What is protected internal?
86. What is private protected?
87. What is encapsulation example?
88. What is abstraction example?
89. What is polymorphism example?
90. What is inheritance example?
91. What is object initializer?
92. What is method hiding?
93. What is new keyword?
94. What is partial class?
95. What is nested class?
96. What is static class?
97. What is dependency inversion?
98. What is SOLID principle?
99. Composition vs inheritance?
100. What is association?
101. What is cohesion?
102. What is coupling?
103. What is immutable object?
104. What is init keyword?
105. What is with expression?
106. What is shallow copy?
107. What is deep copy?
108. What is cloning?
109. What is ICloneable?
110. What is object equality?
111. Equals vs ==?
112. GetHashCode usage?
113. What is indexer?
114. What is the difference between an interface and an abstract class?
115. Can an interface contain fields? Why not?
116. What is the difference between public, private, protected, internal?
117. Difference between method overloading and overriding?
118. What is a sealed class?
119. What is shallow copy vs deep copy?
120. What is the Startup class?
121. TPT/TPC/TPH inheritance mapping and trade-offs?
122. Handle large object graphs and partial updates (PATCH/DTOs)?

## 4. Collections, Iterators & Generics

**113 distinct questions**

1. What is Array?
2. What is ArrayList?
3. List<T>?
4. Dictionary<TKey,TValue>?
5. What is Hashtable?
6. Queue<T>?
7. Stack<T>?
8. LinkedList<T>?
9. HashSet<T>?
10. SortedSet<T>?
11. Concurrent collections?
12. What is ReadOnlyCollection?
13. Collection interfaces?
14. What is IEnumerable?
15. What is ICollection?
16. What is IList?
17. IDictionary?
18. Difference between List and Array?
19. Dictionary vs Hashtable?
20. Collection performance?
21. What are generics?
22. Benefits of generics?
23. Generic classes?
24. Generic methods?
25. What are generic constraints?
26. where T : class?
27. where T : struct?
28. where T : new()?
29. What is covariance?
30. What is contravariance?
31. What is LINQ to Objects?
32. What is LINQ to XML?
33. What is LINQ to SQL?
34. What is deferred execution?
35. What is covariance and contravariance?
36. Generic type specialization?
37. What are collections in C#?
38. Difference between Array and List?
39. Differences between List and ArrayList?
40. What is Dictionary?
41. What is HashSet?
42. What is SortedList?
43. What is Queue?
44. What is Stack?
45. What is LinkedList?
46. What is ICollection vs IEnumerable?
47. What is IEnumerator?
48. What is IQueryable?
49. What is yield return?
50. What is generic class?
51. What is generic method?
52. Difference between IEnumerable<T> and IQueryable<T>?
53. What are LINQ providers?
54. How does LINQ work internally?
55. What is Expression Tree?
56. What is AsEnumerable?
57. What is AsQueryable?
58. What is Select vs SelectMany?
59. What is Single vs SingleOrDefault?
60. What is First vs FirstOrDefault?
61. Difference between Take and Skip?
62. What is GroupBy?
63. What is Join in LINQ?
64. What is Any vs All?
65. What is Distinct?
66. What is collection?
67. What is List?
68. Array vs List?
69. Difference between Dictionary and Hashtable?
70. What is IReadOnlyCollection?
71. What is generic collection?
72. Why generics?
73. What is type safety?
74. What is boxing avoided in generics?
75. What is generic constraint?
76. What is where keyword?
77. What is T type parameter?
78. What is covariance in generics?
79. What is yield keyword?
80. What is iterator?
81. What is custom collection?
82. What is enumerator?
83. What is MoveNext?
84. What is Current property?
85. What is Reset method?
86. What is concurrent collection?
87. What is thread-safe collection?
88. What is immutable collection?
89. What is collection initializer?
90. What is capacity vs count?
91. What is resizing?
92. What is performance difference?
93. What is lookup complexity?
94. What is hash collision?
95. What is comparer?
96. What is IComparer?
97. What is IEqualityComparer?
98. What is sorting?
99. What is searching?
100. What is binary search?
101. What is linear search?
102. What is filtering?
103. What is projection?
104. What is grouping?
105. What is partitioning?
106. What is flattening?
107. What is union?
108. What is intersection?
109. What is an iterator? Explain yield.
110. What is Generic Host vs Web Host?
111. Streams vs byte arrays in responses—tradeoffs?
112. Guarantee ordering (partitioning/sequence keys)?
113. Difference between queues and topics?

## 5. Delegates, Events, Lambdas & Functional C#

**64 distinct questions**

1. Local functions?
2. What is a delegate?
3. Types of delegates?
4. What is multicast delegate?
5. Action delegate?
6. Func delegate?
7. Predicate delegate?
8. Anonymous methods?
9. Lambda expressions?
10. Expression trees?
11. Events?
12. Event handlers?
13. Event publisher/subscriber?
14. Custom events?
15. Difference between delegate and event?
16. Callback functions?
17. Closures?
18. Captured variables?
19. Event memory leaks?
20. Weak events?
21. Practical use cases?
22. What is delegate?
23. What is Func?
24. What is Action?
25. What is Predicate?
26. What is lambda?
27. What is closure?
28. What is event?
29. Delegate vs event?
30. What is event handler?
31. What is publisher-subscriber?
32. What is callback?
33. What is expression lambda?
34. What is statement lambda?
35. What is capturing variable?
36. What is event keyword?
37. What is custom event?
38. What is EventHandler?
39. What is generic delegate?
40. What is invocation list?
41. What is async delegate?
42. What is BeginInvoke?
43. What is EndInvoke?
44. What is thread delegate?
45. What is signal?
46. What is event aggregator?
47. What is functional programming?
48. What is immutability?
49. What is higher-order function?
50. What is currying?
51. What is partial application?
52. What is chaining?
53. What are delegates?
54. What are Func, Action, and Predicate delegates?
55. What is IActionResult?
56. What is ActionResult?
57. What is an action filter?
58. Event schema versioning over time?
59. Mitigate hot partitions in event streams?
60. Prevent retry storms?
61. Invalidate caches safely (token/version/event-driven)?
62. Prevent caching sensitive data?
63. Design replay for event-driven systems?
64. Prevent brute-force attacks?

## 6. LINQ & Expression Trees

**60 distinct questions**

1. What is LINQ?
2. Benefits of LINQ?
3. LINQ architecture?
4. What is LINQ to Entities?
5. Query syntax?
6. Method syntax?
7. Select()?
8. Where()?
9. OrderBy()?
10. GroupBy()?
11. Join()?
12. GroupJoin()?
13. SelectMany()?
14. First() vs FirstOrDefault()?
15. Single() vs SingleOrDefault()?
16. Any()?
17. All()?
18. Count()?
19. What is immediate execution?
20. IQueryable vs IEnumerable?
21. LINQ performance?
22. What is lazy loading?
23. What is eager loading?
24. What is explicit loading?
25. Why LINQ?
26. LINQ syntax types?
27. Query syntax vs method syntax?
28. What is Select?
29. What is Where?
30. What is OrderBy?
31. What is ThenBy?
32. What is Join?
33. What is GroupJoin?
34. What is SelectMany?
35. What is First?
36. What is FirstOrDefault?
37. What is Single?
38. What is SingleOrDefault?
39. What is Any?
40. What is All?
41. What is Count?
42. What is Sum?
43. What is Min?
44. What is Max?
45. What is Average?
46. What is Intersect?
47. What is Except?
48. What is Skip?
49. What is Take?
50. What is pagination?
51. IEnumerable vs IQueryable?
52. What is compiled query?
53. What is transformation?
54. What is performance impact?
55. What is optimization?
56. What is debugging LINQ?
57. What is the difference between IEnumerable and IQueryable?
58. How to implement pagination in Web APIs?
59. Pagination patterns (cursor vs offset)?
60. Limit memory usage on large queries (paging, streaming, projection)?

## 7. Exception Handling & Error Management

**64 distinct questions**

1. What is exception handling?
2. try-catch block?
3. What is finally block?
4. throw keyword?
5. What is throw vs throw ex?
6. What are custom exceptions?
7. Exception filters?
8. What is AggregateException?
9. What is InnerException?
10. What is StackTrace?
11. What is global exception handling?
12. Checked and unchecked?
13. Overflow exceptions?
14. Best practices for exceptions?
15. When should exceptions not be used?
16. What is using statement?
17. What is try-catch?
18. Can finally block skip execution?
19. What is the exception hierarchy?
20. What is TaskCancelledException?
21. What is NullReferenceException?
22. What is InvalidOperationException?
23. What is ArgumentNullException?
24. What is ArgumentException?
25. What is FormatException?
26. What is FileNotFoundException?
27. What is exception filtering?
28. What is UnhandledException?
29. What is AppDomain exceptions?
30. What is `Environment.FailFast`?
31. What is stack overflow exception?
32. What is OutOfMemoryException?
33. When not to use exceptions?
34. What is rethrowing an exception?
35. What is FaultException?
36. What is ExceptionDispatchInfo?
37. What is error logging?
38. What is retry logic?
39. What is exception?
40. What is try block?
41. What is catch block?
42. What is throw?
43. What is throw ex?
44. Difference between throw and throw ex?
45. What is custom exception?
46. What is Exception class?
47. What is stack trace?
48. What is inner exception?
49. What is AppDomain exception?
50. What is dispose?
51. Finalize vs Dispose?
52. What is resource cleanup?
53. What is fail-fast?
54. What is logging?
55. What is fallback?
56. What is exception filter?
57. What is when keyword?
58. What is rethrow?
59. What is aggregate exception?
60. What is task exception?
61. What is unhandled exception?
62. What is best practice?
63. Centralize exception handling in Web API?
64. How does .NET handle exception cost internally?

## 8. Async, Multithreading & Concurrency

**129 distinct questions**

1. What is a thread?
2. Thread lifecycle?
3. Thread class?
4. What is ThreadPool?
5. What is Task Parallel Library (TPL)?
6. Task vs Thread?
7. async and await?
8. What is synchronization?
9. lock statement?
10. What is Mutex?
11. What is Semaphore?
12. SemaphoreSlim?
13. What is Monitor?
14. What is Interlocked?
15. What is deadlock?
16. What is race condition?
17. What is CancellationToken?
18. What is Parallel.For?
19. What is PLINQ?
20. What is asynchronous programming?
21. async keyword?
22. await keyword?
23. What is Task?
24. Task<T>?
25. What is ValueTask?
26. What is ConfigureAwait(false)?
27. What is async streams?
28. What is IAsyncEnumerable?
29. Async exception handling?
30. ValueTask optimization?
31. ThreadPool internals?
32. Task Scheduler architecture?
33. async/await state machine?
34. Deadlock troubleshooting?
35. Race conditions?
36. Lock contention?
37. SemaphoreSlim use cases?
38. Channels in .NET?
39. Producer-consumer patterns?
40. TPL internals?
41. PLINQ optimization?
42. CancellationToken architecture?
43. SynchronizationContext?
44. High throughput processing?
45. What is thread starvation?
46. Parallel system design?
47. What is multithreading?
48. What is async/await?
49. What is lock keyword?
50. What is Monitor class?
51. Difference between Semaphore and SemaphoreSlim?
52. What is AutoResetEvent?
53. What is ManualResetEvent?
54. What is ConfigureAwait?
55. What is thread affinity?
56. What is synchronization context?
57. What is Parallel LINQ (PLINQ)?
58. What is ConcurrentDictionary?
59. What is ConcurrentQueue?
60. What is ConcurrentBag?
61. What is BlockingCollection?
62. What is Task.Run?
63. What is async void?
64. Why async void is dangerous?
65. What is context switching?
66. What is a background thread?
67. What is a foreground thread?
68. What is thread-safe code?
69. What is lock-free programming?
70. What is memory barrier?
71. What is Interlocked class?
72. What is TaskCompletionSource?
73. What is Parallel.Invoke?
74. What is WaitAll vs WhenAll?
75. What is Task.Wait?
76. What is Task.Result?
77. Difference between Task and Thread?
78. What is async stream?
79. What is producer-consumer pattern?
80. What is reactive programming?
81. What is Rx.NET?
82. What is IObservable?
83. What is IObserver?
84. What is TPL Dataflow?
85. What is thread?
86. What is process?
87. Thread vs process?
88. What is async?
89. What is await?
90. What is parallel programming?
91. What is Parallel LINQ?
92. What is lock?
93. What is thread safety?
94. What is volatile?
95. What is cancellation token?
96. What is async Task?
97. What is thread pool?
98. What is starvation?
99. What is fairness?
100. What is blocking?
101. What is non-blocking?
102. What is reactive system?
103. What is event loop?
104. What is concurrency?
105. What is parallelism?
106. Difference between concurrency and parallelism?
107. What is CPU-bound?
108. What is IO-bound?
109. What is scalability?
110. What is performance tuning?
111. What is profiling?
112. What is debugging threads?
113. What is await foreach?
114. What is common pitfalls?
115. What is monitoring?
116. Explain thread vs task.
117. What is deadlock in async?
118. Handle concurrency (rowversion, concurrency tokens)?
119. Troubleshoot thread pool starvation?
120. How async/await affects memory?
121. How does the ThreadPool work internally?
122. What is a deadlock and how to avoid it?
123. Semaphore vs mutex?
124. Async I/O vs CPU-bound tasks?
125. Parallel.ForEach—when to use?
126. What is System.Threading.Channels and channels usage?
127. Avoid thread pool exhaustion?
128. Safely cache async results?
129. Difference between Task.Run and async I/O?

## 9. Memory Management, GC & Resource Management

**108 distinct questions**

1. What is ref struct?
2. What is Garbage Collection?
3. Generations in GC?
4. GC roots?
5. Managed memory?
6. Unmanaged memory?
7. What is IDisposable?
8. Finalizers?
9. What is dispose pattern?
10. What is WeakReference?
11. Memory leaks?
12. What is LOH (Large Object Heap)?
13. What is GC.Collect()?
14. What is memory profiling?
15. Best practices?
16. What is Span<T>?
17. What is Memory<T>?
18. ReadOnlySpan<T>
19. What is unsafe code?
20. What is BenchmarkDotNet?
21. Stack vs Heap internals?
22. GC architecture?
23. What are GC generations?
24. Workstation vs Server GC?
25. Background GC?
26. Sustained low latency GC?
27. LOH internals?
28. POH (Pinned Object Heap)?
29. Memory fragmentation?
30. What is finalization queue?
31. Memory leaks in managed code?
32. WeakReference use cases?
33. Span<T> internals?
34. Memory<T> architecture?
35. ArrayPool<T>?
36. Object pooling strategies?
37. High allocation troubleshooting?
38. BenchmarkDotNet usage?
39. Memory profiling techniques?
40. What is Gen 0?
41. What is Gen 1?
42. What is Gen 2?
43. What is ephemeral segment?
44. What is memory leak in C#?
45. Can managed code leak memory?
46. What is finalize?
47. Difference between Dispose & Finalize?
48. How GC works internally?
49. Why GC.Collect() should not be used?
50. What is Memory Pressure?
51. What is pinned memory?
52. What is SafeHandle?
53. What is stackalloc?
54. What is fixed keyword?
55. What is value task allocation?
56. What is stack vs heap performance?
57. What is array pooling?
58. What is object pooling?
59. What is SOH?
60. What is Gen 0,1,2?
61. What is LOH?
62. What is memory allocation?
63. What is stack allocation?
64. What is heap allocation?
65. What is reference tracking?
66. What is GC root?
67. What is memory leak?
68. What is unmanaged resource?
69. What is pinning?
70. What is GC.Collect?
71. Should you call GC manually?
72. What is weak reference?
73. What is strong reference?
74. What is safe handle?
75. What is span?
76. What is pooling?
77. What is object reuse?
78. What is allocation cost?
79. What is boxing overhead?
80. What is struct optimization?
81. What is cache locality?
82. What is GC pause?
83. What is throughput?
84. What is latency?
85. What is dotMemory?
86. What is dotTrace?
87. What is memory dump?
88. What is diagnostics tool?
89. What is performance counter?
90. What is benchmark?
91. What is allocation-free coding?
92. What is struct vs class memory?
93. What is large object heap?
94. What is fragmentation?
95. What is compaction?
96. What is tuning GC?
97. What is server GC?
98. What is workstation GC?
99. What is GC modes?
100. Design id generation in distributed systems?
101. Debug memory leaks in .NET?
102. Capture full GC dumps in production?
103. Explain Generation 0, 1, 2 in GC.
104. How to reduce pressure on LOH?
105. GC Server vs GC Workstation mode?
106. Detect memory leaks in .NET?
107. What causes Gen 2 GC spikes?
108. Stack-allocated structures (Span, stackalloc)?

## 10. .NET Runtime, CLR & Advanced C# Internals

**44 distinct questions**

1. Pointers in C#?
2. Source Generators?
3. Roslyn Compiler?
4. Dynamic Language Runtime?
5. Generic math?
6. Interceptors (future features)?
7. Native AOT?
8. Explain CLR architecture.
9. How does JIT compilation work?
10. What are Tiered Compilations?
11. RyuJIT vs Legacy JIT?
12. What happens when a C# program starts?
13. CLR Loader process?
14. Assembly loading sequence?
15. Strong-named assemblies?
16. AssemblyLoadContext?
17. Reflection loading issues?
18. IL generation process?
19. Metadata tables?
20. How does the CLR execute methods?
21. Method dispatch mechanisms?
22. Virtual method table (VTable)?
23. Runtime code generation?
24. Native AOT benefits and limitations?
25. What is ReadyToRun compilation?
26. Runtime diagnostics tools?
27. How do you analyze CLR crashes?
28. DLR architecture?
29. Roslyn compiler architecture?
30. Interceptors concepts?
31. Ref structs?
32. Unsafe code scenarios?
33. Pointers in enterprise apps?
34. Custom awaiters?
35. What is the runtime host?
36. What is NativeAOT?
37. What is source generator?
38. What is CoreCLR?
39. Explain JIT vs AOT.
40. Exponential backoff + jitter best practices?
41. Fail fast vs graceful degradation?
42. Implement auditing with interceptors?
43. Difference between JIT, EconoJIT and NGen?
44. What is Tiered Compilation?

## 11. Reflection, Attributes, Serialization & I/O

**24 distinct questions**

1. What is Reflection?
2. Uses of Reflection?
3. Assembly loading?
4. Type metadata?
5. Custom attributes?
6. Built-in attributes?
7. AttributeUsage?
8. Dynamic object creation?
9. Reflection performance?
10. Reflection vs source generators?
11. File class?
12. Directory class?
13. Stream classes?
14. StreamReader?
15. StreamWriter?
16. Binary serialization?
17. JSON serialization?
18. XML serialization?
19. System.Text.Json?
20. Serialization attributes?
21. What is attribute?
22. What is custom attribute?
23. Benefits of ApiController attribute?
24. Pitfalls in System.Text.Json serialization?

## 12. Dependency Injection & Application Infrastructure

**12 distinct questions**

1. What is Dependency Injection?
2. Benefits of DI?
3. Constructor injection?
4. Property injection?
5. Method injection?
6. Service lifetimes?
7. What is scoped?
8. What is transient?
9. File-scoped namespaces?
10. What is Dependency Injection in .NET Core?
11. What is service lifetime?
12. What is service lifetime issue?

## 13. ASP.NET Core, Web API & Communication

**105 distinct questions**

1. What is ASP.NET Core?
2. What is middleware?
3. What is routing?
4. Dependency Injection in ASP.NET Core?
5. Controllers?
6. Action methods?
7. What is model binding?
8. What is filters?
9. What is authentication?
10. What is authorization?
11. JWT Authentication?
12. What is REST API?
13. API Versioning?
14. Minimal APIs?
15. Swagger/OpenAPI?
16. Request pipeline internals?
17. Middleware architecture?
18. Endpoint routing internals?
19. Model binding internals?
20. Filters execution order?
21. Authentication flow?
22. Authorization policies?
23. JWT architecture?
24. OpenID Connect flow?
25. OAuth2 grant types?
26. API versioning strategy?
27. Minimal APIs design?
28. Kestrel internals?
29. HTTP/2 support?
30. HTTP/3 benefits?
31. Rate limiting architecture?
32. Response caching?
33. What is output caching?
34. SignalR architecture?
35. High-scale Web API design?
36. What is API gateway?
37. What are middleware components?
38. What is Kestrel?
39. What is minimal API?
40. What is endpoint routing?
41. What is MVC?
42. HTTP GET vs POST vs PUT vs DELETE?
43. What is model validation?
44. What is dependency injection in ASP.NET?
45. What is IHttpClientFactory?
46. What is CORS?
47. What is authentication vs authorization?
48. What is JWT?
49. What is claims-based identity?
50. What is Swagger?
51. What is OpenAPI?
52. What is versioning in APIs?
53. What is rate limiting?
54. What is caching?
55. What is distributed cache?
56. What is response compression?
57. What is SignalR?
58. What is gRPC?
59. What is WebSockets?
60. What is health check middleware?
61. What is OData?
62. Explain Kestrel web server.
63. What are Middlewares?
64. What is gRPC in .NET Core?
65. What is MVC pattern?
66. How routing works in MVC?
67. What is attribute routing?
68. Difference between conventional vs attribute routing?
69. Explain filters in MVC.
70. How file uploads work in MVC?
71. How do you handle exceptions in MVC?
72. What are middleware differences vs filters?
73. How to secure MVC application?
74. What are cookie-based authentication?
75. Key differences between MVC Controllers and API Controllers in ASP.NET Core?
76. Model binding for complex vs simple types in Web API?
77. Enable and configure CORS policies?
78. Global filters vs middleware vs per-action filters?
79. Implement rate limiting or throttling in ASP.NET Core?
80. API versioning strategies (URL, header, query)?
81. API versioning (semantic vs date-based)?
82. Document APIs effectively (OpenAPI/Swagger)?
83. Role-based vs policy-based authorization?
84. Secure Swagger UI behind authentication?
85. Per-tenant authorization policies?
86. Resource-based authorization handlers?
87. IP allow/deny lists (middleware vs gateway)?
88. What is OpenAPI (Swagger)?
89. Generate OpenAPI docs with Swashbuckle?
90. Annotate controllers/models for OpenAPI?
91. Split a large OpenAPI spec?
92. Document versioned APIs in Swagger?
93. Filter or group endpoints in Swagger UI?
94. Add custom headers and examples to Swagger?
95. Generate client SDKs from OpenAPI and keep in sync?
96. Validate req/resp at runtime against OpenAPI?
97. Publish OpenAPI docs to an API portal?
98. Secure OpenAPI endpoints in production?
99. Maintain backward compatibility of OpenAPI across releases?
100. Choose between REST, gRPC, and async messaging?
101. When prefer gRPC over REST internally?
102. Formalize contracts between services (OpenAPI/proto + CI)?
103. Apply rate limiting to external API calls?
104. What is rate limiting and why do APIs need it?
105. Role-based vs permission-based authorization?

## 14. Entity Framework Core & Data Access

**41 distinct questions**

1. What is EF Core?
2. DbContext?
3. DbSet?
4. Code First vs Database First?
5. Migrations?
6. Change Tracking?
7. EF Core architecture?
8. Change Tracker internals?
9. Query translation pipeline?
10. Expression tree generation?
11. Compiled queries?
12. Tracking vs NoTracking?
13. N+1 problem?
14. Split queries?
15. Global query filters?
16. Interceptors?
17. Value converters?
18. Shadow properties?
19. Concurrency handling?
20. Transactions?
21. Unit of Work pattern?
22. Repository pattern pros/cons?
23. EF performance tuning?
24. Bulk operations?
25. Multi-tenant EF architecture?
26. EF Core pitfalls?
27. Cache EF Core query results safely?
28. How EF Core change tracking works?
29. Trade-offs between NoTracking and tracking queries?
30. Detect and avoid the N+1 query problem?
31. Profile EF Core queries (logs, interceptors, analyzers)?
32. What are compiled queries and when useful?
33. Implement soft deletes and global query filters?
34. Efficient bulk operations considerations?
35. Shadow properties—when to use?
36. Manage migrations across environments?
37. Transactions across multiple DbContexts/resources?
38. DbContext pooling and caveats?
39. Filtered Include and emulation strategies?
40. Tune parameter sniffing issues?
41. Multi-tenancy with EF Core (schema vs discriminator)?

## 15. Design Patterns, SOLID & Clean Architecture

**50 distinct questions**

1. What is singleton?
2. What is repository pattern?
3. What is factory pattern?
4. Abstract Factory Pattern
5. What is builder pattern?
6. Prototype Pattern
7. Adapter Pattern?
8. Facade Pattern
9. Decorator Pattern?
10. Proxy Pattern
11. What is strategy pattern?
12. What is observer pattern?
13. Command Pattern?
14. What is Mediator pattern?
15. Chain of Responsibility
16. State Pattern?
17. Template Method
18. Dependency Injection Pattern
19. What is CQRS?
20. What is unit of work?
21. Explain SOLID principles.
22. Abstract Factory?
23. Event Sourcing?
24. Saga Pattern?
25. Outbox Pattern?
26. Specification Pattern?
27. Repository?
28. Anti-patterns?
29. Real-world pattern selection?
30. What is SOLID?
31. What is SRP?
32. What is OCP?
33. What is LSP?
34. What is ISP?
35. What is DIP?
36. What is prototype?
37. What is facade?
38. What is decorator?
39. What is DI vs IoC?
40. What is TDD?
41. What is unit testing?
42. What is mocking?
43. What is integration testing?
44. What is load testing?
45. What is clean architecture?
46. What is AddSingleton, AddScoped, AddTransient?
47. CQRS benefits vs overkill?
48. Read models for query performance in CQRS?
49. Structure layers in Clean Architecture?
50. CQRS pattern?

## 16. DDD, Microservices, Messaging & Distributed Systems

**84 distinct questions**

1. DDD principles?
2. Ubiquitous language?
3. Bounded Context?
4. Aggregate Root?
5. Entity vs Value Object?
6. Domain Events?
7. Domain Services?
8. Application Services?
9. Anti-Corruption Layer?
10. Context Mapping?
11. Event Storming?
12. Rich vs Anemic Domain Model?
13. DDD in microservices?
14. Aggregate consistency?
15. DDD pitfalls?
16. Why microservices?
17. Monolith vs Microservices?
18. Service boundaries?
19. Database per service?
20. Distributed transactions?
21. Choreography vs Orchestration?
22. What is service discovery?
23. BFF pattern?
24. What is circuit breaker?
25. Retry strategies?
26. Idempotency?
27. Eventual consistency?
28. Service Mesh?
29. Sidecar pattern?
30. Polyglot persistence?
31. Resiliency patterns?
32. Distributed tracing?
33. Production challenges?
34. Message brokers comparison?
35. RabbitMQ architecture?
36. Kafka architecture?
37. Azure Service Bus?
38. Message ordering?
39. Exactly-once delivery?
40. Dead-letter queues?
41. Retry handling?
42. Event-driven architecture?
43. Event contracts?
44. Schema evolution?
45. Message versioning?
46. Event replay?
47. Event sourcing storage?
48. Distributed event processing?
49. What is microservices?
50. What is monolith?
51. What is resilience?
52. Idempotency keys for POST operations—how?
53. Design for eventual consistency?
54. Standardize trace IDs across microservices?
55. Backends for Frontends (BFF) pattern—when?
56. What are API gateways and when to use them?
57. Benefits/trade-offs of microservices vs monoliths?
58. What is the Saga pattern (orchestrated vs choreographed)?
59. Ensure exactly-once or at-least-once semantics?
60. Handle distributed transactions and outbox patterns?
61. Criteria to split a monolith into microservices?
62. Orchestration vs choreography in microservices?
63. Outbox pattern and dual-write prevention?
64. Implement a saga for order processing?
65. Eventual consistency and client communication?
66. Domain event vs integration event?
67. Implement exactly-once with at-least-once infra?
68. Transactional outbox + inbox pattern?
69. What is a service mesh and when to use it?
70. API gateway vs BFF—roles?
71. Multi-tenant microservices (DB-per-tenant vs schema vs shared)?
72. Anti-corruption layer (ACL) and need?
73. Polly resilience policies (retry, circuit breaker, timeout, bulkhead, fallback)?
74. When to use circuit breakers and trigger metrics?
75. Choose idempotency keys and store them?
76. Resilience metrics to track (retries, fallbacks, circuit states)?
77. Map owned entity types and value objects?
78. Distributed transactions without 2PC (sagas/outbox)?
79. Manage schema evolution in messaging (Avro/JSON/proto)?
80. Explain service mesh and problems it solves.
81. Propagate trace IDs across microservices?
82. API Gateway vs Reverse Proxy?
83. What is dead-letter queue and handling?
84. Migrate a large monolith to microservices without downtime—how?

## 17. Docker, Kubernetes, DevOps & Observability

**84 distinct questions**

1. What is IoC container?
2. What is container orchestration?
3. CI/CD pipeline design?
4. What is blue-green deployment?
5. What is canary release?
6. Feature flags?
7. GitOps?
8. Container security?
9. Logging architecture?
10. What is OpenTelemetry?
11. Metrics strategy?
12. SLI/SLO/SLA?
13. Prometheus?
14. Grafana?
15. Incident management?
16. Root cause analysis?
17. What is configuration pipeline?
18. What is logging pipeline?
19. What is self-contained deployment?
20. What is single-file deployment?
21. What is pipeline?
22. What is Serilog?
23. What is deployment?
24. What is Docker?
25. What is containerization?
26. What is CI/CD?
27. What is observability?
28. What is pipeline execution order?
29. How do you use Serilog?
30. Blue/green vs canary releases for microservices?
31. Test microservices integration locally (Testcontainers, compose)?
32. Structure multi-stage YAML pipelines in Azure DevOps/GitHub Actions?
33. Trunk-based development with feature flags and safe deploys?
34. Automate database migrations safely in CI/CD (gates, backups, drift detection)?
35. What is Docker and why for .NET apps?
36. Difference between a container and a VM?
37. Docker images vs containers?
38. Explain Dockerfile structure.
39. What is multi-stage Docker build and why?
40. Reduce Docker image size for .NET apps?
41. What is Docker Compose and dev usage?
42. How to mount volumes in Docker?
43. Pass environment variables securely to containers?
44. Debug .NET code inside containers?
45. Configure networking between multiple containers?
46. Run EF Core migrations in Dockerized envs?
47. Troubleshoot container startup failures?
48. Use docker logs effectively?
49. Healthcheck instruction in Dockerfile?
50. Proper use of .dockerignore?
51. Scan Docker images for vulnerabilities?
52. What is a distroless container?
53. Secure secrets inside containers?
54. Docker layering and caching?
55. Manage configuration across environments in containers?
56. Handle file permissions in Linux containers?
57. Local dev with Docker Compose tools?
58. Linux containers vs Windows containers?
59. Optimize .NET Core app startup time in a container?
60. What is Kubernetes and why?
61. What is a Deployment?
62. What is a ReplicaSet?
63. Deployment vs StatefulSet?
64. What is a DaemonSet?
65. What is a Service in K8s?
66. What is an Ingress controller?
67. How do ConfigMaps work?
68. PersistentVolume vs PersistentVolumeClaim?
69. What is a canary deployment?
70. Pod eviction—troubleshooting?
71. Role of etcd in K8s?
72. Secure Pod-to-Pod communication?
73. Use Kubernetes Operators?
74. Minikube vs Kind vs Docker Desktop K8s?
75. Logging from apps running in K8s?
76. What is a sidecar container and use cases?
77. What is distributed tracing and why important?
78. Explain Serilog and benefits?
79. Capture metrics from .NET apps (Prometheus)?
80. Build dashboards (Grafana, Kibana, App Insights)?
81. What is APM?
82. Test observability in CI/CD?
83. Ensure zero-downtime deployments in App Service?
84. Implement distributed tracing across cloud services?

## 18. Cloud Architecture, Security & Reliability

**97 distinct questions**

1. Azure architecture principles?
2. AWS architecture principles?
3. Multi-cloud strategy?
4. Azure Functions?
5. Durable Functions?
6. Kubernetes architecture?
7. AKS/EKS?
8. Sidecars?
9. Autoscaling?
10. Infrastructure as Code?
11. Terraform architecture?
12. Bicep?
13. Distributed caching?
14. Global load balancing?
15. CDN architecture?
16. What is disaster recovery?
17. Multi-region deployment?
18. OWASP Top 10?
19. SQL Injection prevention?
20. XSS prevention?
21. CSRF mitigation?
22. JWT vulnerabilities?
23. OAuth2 security?
24. What is OpenID Connect?
25. API security?
26. Certificate management?
27. Encryption at rest?
28. Encryption in transit?
29. Key Vault usage?
30. Secrets rotation?
31. Zero Trust Architecture?
32. Security architecture review?
33. What is OAuth?
34. What is encryption?
35. What is Azure?
36. What is AWS?
37. What is cloud computing?
38. What is CSProj vs project.json?
39. OAuth 2.0 roles (resource owner, client, resource server, auth server)?
40. What is JWT and its structure?
41. Common JWT pitfalls (audience, TTLs)?
42. Validate JWTs in ASP.NET Core?
43. Protect against CSRF/XSS/SSRF?
44. Protect secrets in ASP.NET Core (Key Vault, user secrets)?
45. HTTPS enforcement and HSTS?
46. Certificate-based authentication between services?
47. Secure storage & usage of API keys?
48. Symmetric vs asymmetric signing for JWTs?
49. Expose multiple security schemes (JWT, API Key) in Swagger?
50. Choosing a message broker (Kafka/RabbitMQ/Azure Service Bus)?
51. Retry-on-failure for transient errors (SQL Azure)?
52. Use FromSqlRaw safely and prevent SQL injection?
53. Retry with backoff in consumers (Service Bus/DLQ)?
54. Infrastructure as Code (Bicep/Terraform) for .NET solutions?
55. Environment-specific configurations and secrets (Key Vault, variable groups)?
56. What is cloud-native architecture?
57. What is the shared responsibility model in cloud?
58. Compare Azure App Service vs AKS vs Azure Functions.
59. What is Azure API Management and when to use it?
60. Secure secrets using Azure Key Vault?
61. What is Managed Identity and usage?
62. Event Grid vs Service Bus vs Event Hub?
63. Handle message ordering in Service Bus?
64. Implement distributed caching in Azure?
65. Azure Redis Cache vs Memcached?
66. What is Azure Front Door and when needed?
67. Load Balancer vs Application Gateway?
68. What is CDN and how it speeds up APIs?
69. What is an Availability Zone?
70. Explain Azure B2C authentication.
71. Manage configuration using Azure App Configuration?
72. Handle database failover in cloud?
73. Cloud-native logging options (App Insights, CloudWatch)?
74. SNS vs SQS in AWS—differences?
75. AWS Lambda vs Azure Functions—compare.
76. Design event-driven systems in cloud?
77. Compare ARM/Bicep vs Terraform.
78. What is OWASP Top 10 and why important?
79. Prevent SQL injection in .NET applications?
80. What is CSRF?
81. What is XSS and how to mitigate it?
82. What is HSTS and why critical?
83. Data encryption at rest vs in transit?
84. Rotate keys or certificates—how?
85. What is DDoS protection?
86. What is SQL AlwaysEncrypted?
87. Securely store API keys?
88. What is OAuth token introspection?
89. What is SSO (Single Sign-On)?
90. What is SAML and how it differs from OAuth?
91. What is a JWT Kid header?
92. What is mutual TLS and where required?
93. What is the Zero Trust model?
94. RBAC vs ABAC?
95. What is a security penetration test?
96. What is a nonce and where used?
97. What is CSP (Content Security Policy)?

## 19. System Design & Performance Engineering

**28 distinct questions**

1. Design a payment system.
2. Design an order management system.
3. Design Uber-like system.
4. Design Netflix-like streaming.
5. Design URL shortener.
6. Design notification service.
7. Design inventory platform.
8. Design booking platform.
9. Design audit logging system.
10. Design fraud detection system.
11. Design document management system.
12. Design file upload service.
13. Design real-time chat.
14. Design search engine.
15. Design API Gateway.
16. Design caching layer.
17. Design rate limiter.
18. Design distributed cache.
19. Design multi-region architecture.
20. Design high-availability systems.
21. Design a bulk API endpoint?
22. Design a permission model (role, permission, resource, action)?
23. What is distributed cache and hook up Redis?
24. Design multi-region failover systems?
25. Design an API that handles millions of daily transactions—ensure scalability?
26. Design a resilient payment system—key components and flows?
27. Design a multi-tenant SaaS architecture—data and isolation strategies?
28. Design a high-availability global application with zero downtime?

## 20. Testing, Leadership & Architecture Governance

**42 distinct questions**

1. What makes a good software architect?
2. Architecture decision records?
3. Technical debt management?
4. Legacy modernization?
5. Strangler Fig Pattern?
6. Build vs Buy decisions?
7. Architectural trade-offs?
8. CAP theorem?
9. PACELC theorem?
10. Scalability strategies?
11. Availability vs consistency?
12. Horizontal scaling?
13. Vertical scaling?
14. Caching strategies?
15. Read replicas?
16. Database sharding?
17. Multi-tenancy models?
18. Data governance?
19. Architecture reviews?
20. Technical roadmap planning?
21. Engineering governance?
22. Team topology?
23. Conway's Law?
24. Stakeholder management?
25. Managing architecture risks?
26. Architecture KPIs?
27. Cost optimization?
28. Cloud FinOps?
29. High-performance architecture?
30. Enterprise integration patterns?
31. Regulatory compliance architecture?
32. PCI-DSS considerations?
33. HIPAA considerations?
34. GDPR architecture?
35. AI integration architecture?
36. Platform engineering?
37. Enterprise architecture frameworks?
38. How would you modernize a 20-year-old .NET application?
39. Describe the most complex architecture you have designed and defend every decision.
40. What is testing?
41. What is technical debt?
42. Test resilience (chaos testing, fault injection)?

## Suggested Preparation Order

1. C# fundamentals, types, operators, control flow, methods and OOP
2. Collections, generics, delegates, events and LINQ
3. Exception handling, async/await, threading and memory/GC
4. CLR/runtime internals, advanced C# and performance
5. Dependency injection, ASP.NET Core, Web API and EF Core
6. SOLID, design patterns, clean architecture and DDD
7. Microservices, messaging, resilience and distributed systems
8. Docker, Kubernetes, DevOps, observability and cloud
9. Security, system design, performance engineering and leadership

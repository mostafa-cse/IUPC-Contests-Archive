# APM

**URL:** https://toph.co/p/apm  

---

You will be requested to add a new package with a dependent package name list. If there is no conflict to resolve recursive dependencies and all dependent packages do exist in the APM server, then the requested package will be added to the server, otherwise not.

The APM package name formatting is:

package-id:version-number

Example: acm-server:v1.0
                 Here,  package-id = acm-server
                        version-number = v1.0

APM follows transitive dependency rules to resolve dependencies. If package B depends on package C and C depends on D, then B indirectly depends on D.

While adding a new package, dependencies will be conflicted or error will occur if any of the following is true:

if there’s any directly or indirectly dependent package with same package id but different version number

if any of the dependent package doesn’t exist in APM Server

This is a conflicting case, because A:v1.0 wants to import different versions of D.

Input

You are given list of

$N$

(

$1 \le N \le 100$

) requests. Each request has a new package with unique name

$P$

(

$1 \le length(P) \le 100$

) and

$M$

(

$0 \le M \le 10$

) size of the dependent package name list. Then following

$M$

lines contain dependent package names. In a package name, package-id and version number is separated by a colon(:) and contains only alphanumeric characters. Initially APM server contains no package.

Output

For each request find out if there is any error or conflict to add new package. If so, output “Request {ID}: ERROR”, otherwise output "Request {ID}: OK” and print list of all added package names so far including the current one. The list should be ordered lexicographically by package-id, and in case package-id is same, ordered lexicographically by version-number.

Example


---

## Samples

### Sample Input 1
```
7
D:v1.0
0
D:v2.0
0
C:v1.0
1
D:v2.0
B:v1.0
1
D:v1.0
A:v1.0
2
B:v1.0
C:v1.0
E:v1.0
1
C:v1.0
E:v2.0
1
F:v1.0
```

### Sample Output 1
```
Request 1: OK
D:v1.0
Request 2: OK
D:v1.0
D:v2.0
Request 3: OK
C:v1.0
D:v1.0
D:v2.0
Request 4: OK
B:v1.0
C:v1.0
D:v1.0
D:v2.0
Request 5: ERROR
Request 6: OK
B:v1.0
C:v1.0
D:v1.0
D:v2.0
E:v1.0
Request 7: ERROR
```

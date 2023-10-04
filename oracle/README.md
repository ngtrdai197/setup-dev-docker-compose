
# Setup
- Visit page https://container-registry.oracle.com/
- After that, need to register new an account and login
- Select oracle db enterprise or something else
- Look right side and select language -> and continue to read terms of Oracle -> Accept
- We need login to registry hub of Oracle to request permission.
```bash
docker login container-registry.oracle.com
```
- And then, we have permission and we can pull oracle image:
```bash
docker pull container-registry.oracle.com/database/enterprise:12.2.0.1
```
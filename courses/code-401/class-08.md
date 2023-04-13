# Code 401 Reading 7

## 5 steps to RBAC

### What is Role Based Access Control (RBAC) and why do we care?

Role based access control is assigning system access to users based on their role in an organization

- users get roles based on job responsibilities
- users get access based on roles

### Describe a Role/Permission heirarchy that you might implement using RBAC

- admins = people who need root/admin access. sys admins only
- push access = developers authorized to push code to production. team leads?
- write access = developers authorized to write/edit code
- limited users = people who need access to productivity software only, HR etc

### What approach might you take to implement RBAC?

- Identify what the roles are
- Identify what they need to be able to do in the system
- Assign roles to employees
- If employees need different access, reassign them to new role
- Don't assign roles to people who don't need them

## wiki - RBAC

### If Authentication is “you are who you say you are,” what is Authorization?

Authorization = are you allowed to access a resource? yes = authorized

### Name three primary rules defined for RBAC

1. Role assignment, can have permission only if assigned that role
2. Role authorization, active role must be authorized
3. Permission authorization, permission must be authorized for active role

### Describe RBAC to a non-technical friend

Role based authorization is a way of dividing up access to computer systems based on what the employees/organizaton members actually do

It means defining which jobs/roles need access to what things

Then it means don't let people whose job doesn't involve something have access to it

## Video - RBAC tutorial

### What Are access rights Associated with? The User? or The Role? Explain

### Access Rights, or Authorization, is activated after a user successfully does what?

### Explain how RBAC might benefit a business

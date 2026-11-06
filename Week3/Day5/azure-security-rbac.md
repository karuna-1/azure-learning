# Day 5 – Azure Security and RBAC

## 1. Azure RBAC

RBAC stands for Role-Based Access Control.

It controls who can access Azure resources and what actions they can perform.

## 2. Common Azure Roles

- Owner: Full access, including assigning permissions.
- Contributor: Can create, update, and delete resources but cannot assign roles.
- Reader: Can only view resources.

## 3. Principle of Least Privilege

Give users only the permissions they need to perform their tasks.

This improves security and reduces accidental changes.

## 4. Managed Identity

Managed Identity allows Azure resources to authenticate to supported Azure services without storing credentials in application code.

### Types

- System-assigned: Created and managed with an Azure resource.
- User-assigned: Created separately and can be attached to multiple resources.

## 5. Why Azure Security Matters

- Protects sensitive data.
- Controls resource access.
- Reduces unauthorized access.
- Avoids storing credentials in code.

## Key Takeaway

Use RBAC to control permissions and Managed Identity to authenticate Azure resources securely.
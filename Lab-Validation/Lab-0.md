# Lab 0 - Validation Findings

## Status

* Passed with observations

## Student Experience Findings

### Missing Environment Creation Steps

Current instructions assume the **Dev One** environment already exists.

During testing, the environment was not available until it was manually created.

Add the following steps before Power Apps validation:

1. Open `https://admin.powerplatform.microsoft.com/` in an InPrivate/Incognito window.
2. Sign in using lab credentials.
3. Navigate to **Manage** > **+ New**.
4. Create a new environment:

   * Type: **Trial**
   * Region: **UAE**
   * Name: **Dev One [YourName]**
   * Enable **Dataverse (Add Dataverse data store)**
5. Select **Next**.
6. Configure Dataverse:

   * Language: **English (US)**
   * Currency: **AED**
   * Security Group: **None**
7. Select **Done** and **Save**.
8. Wait for environment provisioning to complete.
9. Verify **Dev One [YourName]** is available before continuing.

### Missing MFA Guidance

First-time sign-in required:

* Password reset
* Microsoft Authenticator registration

Add note:

> First-time sign in may require password reset and Microsoft Authenticator MFA registration before Power Apps can be accessed.

### Environment Provisioning Note

Environment creation is not immediate.

Add note:

> Environment provisioning may take several minutes. Wait until the environment status is ready before continuing.

### Typo

Current:

```text
Trail
```

Suggested:

```text
Trial
```

## Impact

Without environment creation instructions, students may be unable to locate the expected **Dev One** environment and may assume tenant configuration issues.

## Recommendation

The lab instruction document requires updates to include:

- Environment creation steps
- Microsoft Authenticator setup guidance
- Environment provisioning note
- Correction of typo: Trail → Trial

These findings were observed during validation and have not yet been applied to the lab document.
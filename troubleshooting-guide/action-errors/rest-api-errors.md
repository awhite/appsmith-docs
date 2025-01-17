# REST API Errors

![Click to expand](../../.gitbook/assets/api-error.png)

### Missing URL Error

```text
DEFAULT_REST_DATASOURCE is not correctly configured. Please fix the following and then re-run: \n[Missing URL.]
```

This message indicates that the REST API's URL field in the [API editor form](https://docs.appsmith.com/core-concepts/connecting-to-data-sources/connect-to-apis/execute-apis) has been left empty.

This error can be fixed by editing the [REST API form](https://docs.appsmith.com/core-concepts/connecting-to-data-sources/connect-to-apis/execute-apis) and providing a URL.

### Missing Client Secret / Client ID / Access Token Error

```text
DEFAULT_REST_DATASOURCE is not correctly configured. Please fix the following and then re-run: \n[Missing Client Secret, Missing Client ID, Missing Access Token URL]
```

This message indicates that the mentioned parameter fields - `Client Secret` / `Client ID` / `Access Token URL` have been left empty. These fields are nested in the `Authentication` sub-section which becomes visible if the `Authentication Type` field has been chosen as [OAuth 2.0](https://docs.appsmith.com/core-concepts/connecting-to-data-sources/connect-to-apis/authentication/oauth2-authentication)

### Secret Key Required Error

```text
Secret key is required when sending session details is switched on, and should be at least 32 characters in length.
```

This message indicates that `Send Appsmith signature header` field has been marked as `Yes` but the `Session Details Signature Key` field is left empty.

This error can be resolved by filling in the `Session Details Signature Key` field or by disabling the `Send Appsmith signature header` field by selecting `No`.



# Client Class Documentation

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| http_client_instance | `Union[Session, HttpClientProvider]` | The Http Client passed from the sdk user for making requests |
| override_http_client_configuration | `bool` | The value which determines to override properties of the passed Http Client from the sdk user |
| http_call_back | `HttpCallBack` | The callback value that is invoked before and after an HTTP call is made to an endpoint |
| timeout | `float` | The value to use for connection timeout. <br> **Default: 50** |
| max_retries | `int` | The number of times to retry an endpoint call if it fails. <br> **Default: 0** |
| backoff_factor | `float` | A backoff factor to apply between attempts after the second try. <br> **Default: 2** |
| retry_statuses | `Array of int` | The http statuses on which retry is to be done. <br> **Default: [408, 413, 429, 500, 502, 503, 504, 521, 522, 524, 408, 413, 429, 500, 502, 503, 504, 521, 522, 524]** |
| retry_methods | `Array of string` | The http methods on which retry is to be done. <br> **Default: ["GET", "PUT", "GET", "PUT"]** |
| proxy_settings | [`ProxySettings`](../doc/proxy-settings.md) | Optional proxy configuration to route HTTP requests through a proxy server. |
| logging_configuration | [`LoggingConfiguration`](../doc/logging-configuration.md) | The SDK logging configuration for API calls |
| api_key_credentials | [`ApiKeyCredentials`](auth/custom-header-signature.md) | The credential object for Custom Header Signature |
| bearer_auth_credentials | [`BearerAuthCredentials`](auth/oauth-2-bearer-token.md) | The credential object for OAuth 2 Bearer token |

The API client can be initialized as follows:

## Code-Based Client Initialization

```python
import logging

from webhooksandcallbacksapi.configuration import Environment
from webhooksandcallbacksapi.http.auth.api_key import ApiKeyCredentials
from webhooksandcallbacksapi.http.auth.bearer_auth import BearerAuthCredentials
from webhooksandcallbacksapi.logging.configuration.api_logging_configuration import LoggingConfiguration
from webhooksandcallbacksapi.logging.configuration.api_logging_configuration import RequestLoggingConfiguration
from webhooksandcallbacksapi.logging.configuration.api_logging_configuration import ResponseLoggingConfiguration
from webhooksandcallbacksapi.webhooksandcallbacksapi_client import WebhooksandcallbacksapiClient

client = WebhooksandcallbacksapiClient(
    api_key_credentials=ApiKeyCredentials(
        x_api_key='X-API-Key'
    ),
    bearer_auth_credentials=BearerAuthCredentials(
        access_token='AccessToken'
    ),
    environment=Environment.PRODUCTION,
    logging_configuration=LoggingConfiguration(
        log_level=logging.INFO,
        request_logging_config=RequestLoggingConfiguration(
            log_body=True
        ),
        response_logging_config=ResponseLoggingConfiguration(
            log_headers=True
        )
    )
)
```

## Environment-Based Client Initialization

```python
from webhooksandcallbacksapi.webhooksandcallbacksapi_client import WebhooksandcallbacksapiClient

# Specify the path to your .env file if it’s located outside the project’s root directory.
client = WebhooksandcallbacksapiClient.from_environment(dotenv_path='/path/to/.env')
```

See the [Environment-Based Client Initialization](../doc/environment-based-client-initialization.md) section for details.

## Webhooks and Callbacks API Client

The gateway for the SDK. This class acts as a factory for the Apis and also holds the configuration of the SDK.

## Apis

| Name | Description |
|  --- | --- |
| orders | Gets OrdersApi |


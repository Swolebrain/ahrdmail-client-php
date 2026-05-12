# # SendEmailRequestContent

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**subtenant_id** | **string** |  |
**from** | **string** | A non-empty string that must not contain CR (\\r) or LF (\\n) characters. Applied to all email header fields where injection would be possible. |
**to** | **string[]** | A list of strings where each entry must not contain CR or LF. |
**cc** | **string[]** | A list of strings where each entry must not contain CR or LF. | [optional]
**bcc** | **string[]** | A list of strings where each entry must not contain CR or LF. | [optional]
**reply_to** | **string** | A non-empty string that must not contain CR (\\r) or LF (\\n) characters. Applied to all email header fields where injection would be possible. | [optional]
**in_reply_to** | **string** | A non-empty string that must not contain CR (\\r) or LF (\\n) characters. Applied to all email header fields where injection would be possible. | [optional]
**references** | **string[]** | A list of strings where each entry must not contain CR or LF. | [optional]
**subject** | **string** | A non-empty string that must not contain CR (\\r) or LF (\\n) characters. Applied to all email header fields where injection would be possible. |
**body** | [**\OpenAPI\Client\Model\EmailBody**](EmailBody.md) |  |
**campaign_id** | **string** |  | [optional]
**tags** | **array<string,string>** |  | [optional]
**headers** | **array<string,string>** |  | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)

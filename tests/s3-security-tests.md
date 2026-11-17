## S3 Security Test Results
## Test 01: Anonymous Object Access

Resource: `finance/report.txt`
Test method: Opened the S3 Object URL in an incognito browser window without AWS authentication.

Expected result: AccessDenied

Actual result: AccessDenied

Status: PASS

## Security Finding

Amazon S3 rejected the anonymous request. The test did not expose the object's contents.

## Limitations

This test confirms that one anonymous access attempt was denied. It does not independently verify every bucket permission, IAM policy, or public access configuration.

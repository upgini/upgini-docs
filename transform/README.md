# API Documentation for Transactional Transform Method

## Overview

This document describes the API method for performing a transactional transform using the Upgini endpoint. This endpoint is used to apply transformations based on previously trained features using the FeaturesEnricher model.

## Authentication

To access the endpoint, an API_KEY is required. This key must be the same one used during the training of the FeaturesEnricher.

## Request

The request to the http_inference_trigger endpoint is made using the HTTP POST method. Below is a template for the request using curl:

## Example of request:
```bash
curl "https://search.upgini.com/test/api/http_inference_trigger?search_id=<put search identifier here>" \
    -H "Authorization: <put API_KEY here>" \
    -H "Content-Type: application/json" \
    -d '{"search_keys": {"COUNTRY": {"name": "country_code", "value": "GB"}, "DATE": {"name": "rep_date", "value": "2020-01-01"}, "POSTAL_CODE": {"name": "zip", "value": "111111"}}, "features": {"feature1": "featureValue1", "feature2": "featureValue2}}'
```

## Parameters

* `Authorization`: (Header) The API key (without Bearer).
* `Content-Type`: (Header) Set this to application/json to indicate the type of data being sent.
* `search_id`: (Request param) This is the identifier obtained after initiating the training of the FeaturesEnricher. It should be replaced with the actual search identifier.
* `search_keys`: (Body) A dictionary where the keys are the types of search keys (possible values: PHONE, EMAIL, HEM, COUNTRY, POSTAL_CODE, DATE, IP) used during fit, and the values are the names used for search keys on fit and specific values for these keys.
* `features`: (Body) If features were used during fit to generate new features, they must be specified here with their corresponding values.

## Response

The API response will include the transformed features based on the input data.

Example of successful response:

```json
{
    "status": "ok", 
    "result": {
        "f_enriched_feature1": 18.0,
        "f_autofe_mul_sd8f7s9": 234.4,
        "f_enriched_cat_feature2": "test",
        "f_empty_feature3": null,
        "feature1_bd1088_emb1208": -0.007415670435875654,
        "feature1_bd1088_emb775": 0.03687792643904686,
        "feature2_bd1088_emb99": -0.01887989602982998,
        "feature2_bd1088_emb1172": -0.04251651093363762
    },
    "trace_id": "2d4f48f5-3052-4cdd-b1ec-4a18ea4430cc"
}
```
Set of feature names in result could be different depends on passed search_id.

If some features or all features not found by passed search key or search key is missing on the server side then `null` will be returned as value of features:

```json
{
   "status": "ok",
   "result": {"f_upgini_feature1": null, "f_upgini_feature2": null},
   "traceId": "2d4f48f5-3052-4cdd-b1ec-4a18ea4430cc"
}
```

## Error Handling

In case of errors, the API will return appropriate HTTP status codes (400 - invalid request body structure, 401 - invalid API_KEY, 403 - passed search_id that doesn't belong to the account, 404 - passed search_id of unexisting search, 429 - rate limit exceeded) along with descriptive error messages to help diagnose issues.

Example of failed response:
```json
{
    "status": "error",
    "errorMessage": "Detailed message"
}
```

## Limits

The service has limitation of 10 RPS (request per second) for one account.

## Best Practices

Ensure the API_KEY is kept secure and not exposed in client-side code.
Validate inputs before sending to prevent errors related to data format.
Use HTTPS to ensure the security of data in transit.

## Support

For issues or questions regarding the API, please contact the support team at support@upgini.com.

Please replace placeholders with actual values when constructing your request.

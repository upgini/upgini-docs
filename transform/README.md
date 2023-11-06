# API for transactional transform

Example of request:
```bash
curl "https://inference-upgini.azurewebsites.net/api/http_inference_trigger" \
    -H "Authorization: <put API_KEY here>" \
    -H "Content-Type: application/json" \
    -d '{"search_id": "<put search identifier here>", "search_keys": {"COUNTRY": "GB", "DATE": "2020-01-01", "POSTAL_CODE": "111111"}, "features": {"feature1": "featureValue1", "feature2": "featureValue2}}'
```
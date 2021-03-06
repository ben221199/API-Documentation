# Finsky Digital Front End (FDFE)

The API of Finsky Digital Front End is used to get information about apps from the Google Play Store.

## Headers

| Name | Type | Description |
| --- | --- | --- |
| X-DFE-Client-Id | Request | ... |
| X-DFE-Content-Filters | Request | ... |
| X-DFE-Content-Length | Response | ... |
| X-DFE-Cookie | Request | ... |
| X-DFE-Device-Config-Token | Request | ... |
| X-DFE-Device-Id | Request | ... |
| X-DFE-Encoded-Targets | Request | ... |
| X-DFE-Hard-TTL | Response | ... |
| X-DFE-MCCMNC | Request | ... |
| X-DFE-Network-Type | Request | ... |
| X-DFE-Phenotype | Request | ... |
| X-DFE-Request-Params | Request | ... |
| X-DFE-Soft-TTL | Response | ... |
| X-DFE-UserLanguages | Request | ... |

## Endpoints

Base URL: https://android.clients.google.com/fdfe

### ![GET](https://img.shields.io/badge/GET-green) /details

#### URL Parameters

| Name | Description | Required | Example |
| --- | --- | --- | --- |
| doc | Document you want details of.<br>Can be Developer ID or Package Name. | ... | `developer-5700313618786177705` (Developer ID)<br>`com.google.android.googlequicksearchbox` (Package Name) |

### ![GET](https://img.shields.io/badge/GET-green) /reviewQuestions

doc

### ![GET](https://img.shields.io/badge/GET-green) /getDetailsStream

doc, edsctx

### ![GET](https://img.shields.io/badge/GET-green) /promotion/detailsPagePromotion

doc

### ![GET](https://img.shields.io/badge/GET-green) /reviewSummary

doc

### ![GET](https://img.shields.io/badge/GET-green) /getPostAcquireDetailsStream

doc, edsctx

### ![POST](https://img.shields.io/badge/POST-blue) /apps/contentSync

nocache_qos

### ![GET](https://img.shields.io/badge/GET-green) /searchSuggest

q, nocache_pssi, ssis, sb, sst, nocache_ibr

### ![GET](https://img.shields.io/badge/GET-green) /search

q, c, ksm

### ![GET](https://img.shields.io/badge/GET-green) /api/userProfile


### ![GET](https://img.shields.io/badge/GET-green) /getCluster

enpt, n
(n not required)

### ![GET](https://img.shields.io/badge/GET-green) /searchList

q, o, c, ksm

### ![GET](https://img.shields.io/badge/GET-green) /delivery

doc, ot, st, vc, da, ia, fdcf, isid

### ![GET](https://img.shields.io/badge/GET-green) /getStream

ecp, n

### ![GET](https://img.shields.io/badge/GET-green) /topChartsStream

c, cat

### ![GET](https://img.shields.io/badge/GET-green) /inlineTopCharts

c, cat, dcr

### ![GET](https://img.shields.io/badge/GET-green) /stream

esp, n

### ![GET](https://img.shields.io/badge/GET-green) /cluster

ecp, ctntkn, n, o

### ![GET](https://img.shields.io/badge/GET-green) /getHomeStream

c, cat, ehsctx, n

### ![POST](https://img.shields.io/badge/POST-blue) /myApps

### ![POST](https://img.shields.io/badge/POST-blue) /bulkDetails

### ![GET](https://img.shields.io/badge/GET-green) /popups

### ![POST](https://img.shields.io/badge/POST-blue) /acquire

theme

### ![POST](https://img.shields.io/badge/POST-blue) /moduleDelivery

### ![GET](https://img.shields.io/badge/GET-green) /getBrowseStream

ecp

### ![GET](https://img.shields.io/badge/GET-green) /reviewSummary

doc

### ![GET](https://img.shields.io/badge/GET-green) /reviewQuestions

doc

### ![GET](https://img.shields.io/badge/GET-green) /selfUpdate

susp, nocache_qos

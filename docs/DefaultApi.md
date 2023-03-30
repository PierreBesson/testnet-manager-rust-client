# \DefaultApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_invulnerables_api_collators_para_id_add_invulnerables_post**](DefaultApi.md#add_invulnerables_api_collators_para_id_add_invulnerables_post) | **POST** /api/collators/{para_id}/add_invulnerables | Add Invulnerables
[**deregister_collators_api_collators_para_id_deregister_post**](DefaultApi.md#deregister_collators_api_collators_para_id_deregister_post) | **POST** /api/collators/{para_id}/deregister | Deregister Collators
[**deregister_validators_api_validators_deregister_post**](DefaultApi.md#deregister_validators_api_validators_deregister_post) | **POST** /api/validators/deregister | Deregister Validators
[**get_collators_api_collators_para_id_get**](DefaultApi.md#get_collators_api_collators_para_id_get) | **GET** /api/collators/{para_id} | Get Collators
[**get_node_logs_api_nodes_node_name_logs_get**](DefaultApi.md#get_node_logs_api_nodes_node_name_logs_get) | **GET** /api/nodes/{node_name}/logs | Get Node Logs
[**get_nodes_api_nodes_get**](DefaultApi.md#get_nodes_api_nodes_get) | **GET** /api/nodes | Get Nodes
[**get_nodes_api_nodes_node_name_get**](DefaultApi.md#get_nodes_api_nodes_node_name_get) | **GET** /api/nodes/{node_name} | Get Nodes
[**get_parachains_api_parachains_get**](DefaultApi.md#get_parachains_api_parachains_get) | **GET** /api/parachains | Get Parachains
[**get_runtime_api_runtime_get**](DefaultApi.md#get_runtime_api_runtime_get) | **GET** /api/runtime | Get Runtime
[**get_runtime_configuration_api_runtime_configuration_get**](DefaultApi.md#get_runtime_configuration_api_runtime_configuration_get) | **GET** /api/runtime/configuration | Get Runtime Configuration
[**get_runtime_parachain_api_parachains_para_id_runtime_get**](DefaultApi.md#get_runtime_parachain_api_parachains_para_id_runtime_get) | **GET** /api/parachains/{para_id}/runtime | Get Runtime Parachain
[**get_validators_api_validators_get**](DefaultApi.md#get_validators_api_validators_get) | **GET** /api/validators | Get Validators
[**health_health_get**](DefaultApi.md#health_health_get) | **GET** /health | Health
[**offboard_parachains_api_parachains_offboard_post**](DefaultApi.md#offboard_parachains_api_parachains_offboard_post) | **POST** /api/parachains/offboard | Offboard Parachains
[**onboard_parachains_api_parachains_onboard_post**](DefaultApi.md#onboard_parachains_api_parachains_onboard_post) | **POST** /api/parachains/onboard | Onboard Parachains
[**parachain_upload_runtime_and_upgrade_api_parachains_para_id_runtime_upgrade_post**](DefaultApi.md#parachain_upload_runtime_and_upgrade_api_parachains_para_id_runtime_upgrade_post) | **POST** /api/parachains/{para_id}/runtime/upgrade | Parachain Upload Runtime And Upgrade
[**register_collators_api_collators_para_id_register_post**](DefaultApi.md#register_collators_api_collators_para_id_register_post) | **POST** /api/collators/{para_id}/register | Register Collators
[**register_validators_api_validators_register_post**](DefaultApi.md#register_validators_api_validators_register_post) | **POST** /api/validators/register | Register Validators
[**remove_invulnerables_api_collators_para_id_remove_invulnerables_post**](DefaultApi.md#remove_invulnerables_api_collators_para_id_remove_invulnerables_post) | **POST** /api/collators/{para_id}/remove_invulnerables | Remove Invulnerables
[**rotate_session_keys_api_rotate_session_keys_post**](DefaultApi.md#rotate_session_keys_api_rotate_session_keys_post) | **POST** /api/rotate_session_keys | Rotate Session Keys
[**set_on_chain_keys_api_collators_set_on_chain_keys_post**](DefaultApi.md#set_on_chain_keys_api_collators_set_on_chain_keys_post) | **POST** /api/collators/set_on_chain_keys | Set On Chain Keys
[**teleport_funds_from_sudo_api_xcm_teleport_funds_post**](DefaultApi.md#teleport_funds_from_sudo_api_xcm_teleport_funds_post) | **POST** /api/xcm/teleport_funds | Teleport Funds From Sudo
[**update_runtime_configuration_api_runtime_configuration_post**](DefaultApi.md#update_runtime_configuration_api_runtime_configuration_post) | **POST** /api/runtime/configuration | Update Runtime Configuration
[**upload_runtime_and_upgrade_api_runtime_upgrade_post**](DefaultApi.md#upload_runtime_and_upgrade_api_runtime_upgrade_post) | **POST** /api/runtime/upgrade | Upload Runtime And Upgrade



## add_invulnerables_api_collators_para_id_add_invulnerables_post

> serde_json::Value add_invulnerables_api_collators_para_id_add_invulnerables_post(para_id, address, node)
Add Invulnerables

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**para_id** | **String** | Parachain ID | [required] |
**address** | Option<[**Vec<String>**](String.md)> | Address(es) to be added as invulnerables |  |[default to []]
**node** | Option<[**Vec<String>**](String.md)> | Collator node(s) be added as invulnerables on the parachain |  |[default to []]

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## deregister_collators_api_collators_para_id_deregister_post

> serde_json::Value deregister_collators_api_collators_para_id_deregister_post(para_id, statefulset, node)
Deregister Collators

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**para_id** | **String** | Parachain ID on which to deregister collators | [required] |
**statefulset** | Option<**String**> | Name of the StatefulSet to deregister |  |
**node** | Option<[**Vec<String>**](String.md)> | Name of the node(s) to be deregistered |  |[default to []]

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## deregister_validators_api_validators_deregister_post

> serde_json::Value deregister_validators_api_validators_deregister_post(statefulset, address, node)
Deregister Validators

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**statefulset** | Option<**String**> | Name of the StatefulSet containing the nodes to be deregistered |  |
**address** | Option<[**Vec<String>**](String.md)> | Address(es) to be deregistered |  |
**node** | Option<[**Vec<String>**](String.md)> | Name of the node(s) to be deregistered |  |[default to []]

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_collators_api_collators_para_id_get

> serde_json::Value get_collators_api_collators_para_id_get(para_id, statefulset)
Get Collators

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**para_id** | **String** | ID of the parachain for which to get collators | [required] |
**statefulset** | Option<**String**> | To restrict the displayed nodes to a single StatefulSet |  |[default to ]

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_node_logs_api_nodes_node_name_logs_get

> String get_node_logs_api_nodes_node_name_logs_get(node_name)
Get Node Logs

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**node_name** | **String** | Name of the node | [required] |

### Return type

**String**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: text/plain, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_nodes_api_nodes_get

> serde_json::Value get_nodes_api_nodes_get(statefulset)
Get Nodes

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**statefulset** | Option<**String**> | To restrict the displayed nodes to a single StatefulSet |  |[default to ]

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_nodes_api_nodes_node_name_get

> serde_json::Value get_nodes_api_nodes_node_name_get(node_name)
Get Nodes

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**node_name** | **String** | Name of the node | [required] |

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_parachains_api_parachains_get

> serde_json::Value get_parachains_api_parachains_get()
Get Parachains

### Parameters

This endpoint does not need any parameter.

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_runtime_api_runtime_get

> serde_json::Value get_runtime_api_runtime_get()
Get Runtime

### Parameters

This endpoint does not need any parameter.

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_runtime_configuration_api_runtime_configuration_get

> serde_json::Value get_runtime_configuration_api_runtime_configuration_get()
Get Runtime Configuration

### Parameters

This endpoint does not need any parameter.

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_runtime_parachain_api_parachains_para_id_runtime_get

> serde_json::Value get_runtime_parachain_api_parachains_para_id_runtime_get(para_id)
Get Runtime Parachain

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**para_id** | **String** | ID of the parachain for which to get runtime info | [required] |

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_validators_api_validators_get

> serde_json::Value get_validators_api_validators_get(statefulset)
Get Validators

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**statefulset** | Option<**String**> | To restrict the displayed nodes to a single StatefulSet |  |[default to ]

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## health_health_get

> serde_json::Value health_health_get()
Health

### Parameters

This endpoint does not need any parameter.

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## offboard_parachains_api_parachains_offboard_post

> serde_json::Value offboard_parachains_api_parachains_offboard_post(para_id)
Offboard Parachains

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**para_id** | [**Vec<String>**](String.md) | Parachain ID(s) to offboard | [required] |

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## onboard_parachains_api_parachains_onboard_post

> serde_json::Value onboard_parachains_api_parachains_onboard_post(para_id)
Onboard Parachains

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**para_id** | [**Vec<String>**](String.md) | Parachain ID(s) to onboard | [required] |

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## parachain_upload_runtime_and_upgrade_api_parachains_para_id_runtime_upgrade_post

> serde_json::Value parachain_upload_runtime_and_upgrade_api_parachains_para_id_runtime_upgrade_post(para_id, runtime)
Parachain Upload Runtime And Upgrade

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**para_id** | **String** | Parachain ID on which to upgrade runtime | [required] |
**runtime** | **std::path::PathBuf** | File with runtime: *.compact.compressed.wasm | [required] |

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## register_collators_api_collators_para_id_register_post

> serde_json::Value register_collators_api_collators_para_id_register_post(para_id, statefulset, node)
Register Collators

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**para_id** | **String** | Parachain ID on which to register collators | [required] |
**statefulset** | Option<**String**> | Name of the StatefulSet to register |  |
**node** | Option<[**Vec<String>**](String.md)> | Name of the node(s) to be registered |  |[default to []]

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## register_validators_api_validators_register_post

> serde_json::Value register_validators_api_validators_register_post(statefulset, address, node)
Register Validators

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**statefulset** | Option<**String**> | Name of the StatefulSet containing the nodes to be registered |  |
**address** | Option<[**Vec<String>**](String.md)> | Address(es) to be deregistered |  |[default to []]
**node** | Option<[**Vec<String>**](String.md)> | Name of the node(s) to be registered |  |[default to []]

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## remove_invulnerables_api_collators_para_id_remove_invulnerables_post

> serde_json::Value remove_invulnerables_api_collators_para_id_remove_invulnerables_post(para_id, address, node)
Remove Invulnerables

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**para_id** | **String** | Parachain ID | [required] |
**address** | Option<[**Vec<String>**](String.md)> | Address(es) to removed from invulnerables |  |[default to []]
**node** | Option<[**Vec<String>**](String.md)> | Collator node(s) to be removed as invulnerables on the parachain |  |[default to []]

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## rotate_session_keys_api_rotate_session_keys_post

> serde_json::Value rotate_session_keys_api_rotate_session_keys_post(all, statefulset, node)
Rotate Session Keys

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**all** | Option<**bool**> | Set to true to rotate all nodes session keys |  |[default to false]
**statefulset** | Option<**String**> | Name of the StatefulSet for which to rotate session keys |  |
**node** | Option<[**Vec<String>**](String.md)> | Name of the node(s) for which to rotate session keys |  |[default to []]

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## set_on_chain_keys_api_collators_set_on_chain_keys_post

> serde_json::Value set_on_chain_keys_api_collators_set_on_chain_keys_post(para_id, node, statefulset)
Set On Chain Keys

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**para_id** | **String** | Parachain ID | [required] |
**node** | Option<[**Vec<String>**](String.md)> | Collator node(s) for which to set keys on chain |  |[default to []]
**statefulset** | Option<**String**> | Name of the StatefulSet for which to set keys on chain |  |

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## teleport_funds_from_sudo_api_xcm_teleport_funds_post

> serde_json::Value teleport_funds_from_sudo_api_xcm_teleport_funds_post(para_id, account, amount)
Teleport Funds From Sudo

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**para_id** | **i32** | Parachain ID | [required] |
**account** | [**Vec<String>**](String.md) | Account(s) to fund on the Parachain (in relay-chain SS58 format) | [required] |
**amount** | Option<**i32**> | Amount to transfer to each accounts |  |

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_runtime_configuration_api_runtime_configuration_post

> serde_json::Value update_runtime_configuration_api_runtime_configuration_post(body)
Update Runtime Configuration

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | **serde_json::Value** |  | [required] |

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## upload_runtime_and_upgrade_api_runtime_upgrade_post

> serde_json::Value upload_runtime_and_upgrade_api_runtime_upgrade_post(runtime)
Upload Runtime And Upgrade

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**runtime** | **std::path::PathBuf** | File with runtime: *.compact.compressed.wasm | [required] |

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


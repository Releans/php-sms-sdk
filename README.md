# Getting started

The Releans SDK enables developers to use Releans Services in their code. You can get started in minutes.

```composer require releans/php-client-sdk```

## Initialization

### Authentication
In order to setup authentication and initialization of the API client, you need the following information.

| Parameter | Description |
|-----------|-------------|
| oAuthAccessToken | Your API KEY |



API client can be initialized as following.

```php
$oAuthAccessToken = 'oAuthAccessToken'; // OAuth 2.0 Access Token

$client = new ReleansAPILib\ReleansAPIClient($oAuthAccessToken);
```


# Class Reference

## <a name="list_of_controllers"></a>List of Controllers

* [MessageController](#message_controller)
* [SenderController](#sender_controller)
* [BalanceController](#balance_controller)

## <a name="message_controller"></a>![Class: ](https://apidocs.io/img/class.png ".MessageController") MessageController

### Get singleton instance

The singleton instance of the ``` MessageController ``` class can be accessed from the API Client.

```php
$message = $client->getMessage();
```

### <a name="get_all_messages"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.getAllMessages") getAllMessages

> List all messages sent by the account.


```php
function getAllMessages($accept)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| accept |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$accept = '*/*';

$result = $message->getAllMessages($accept);

```


### <a name="get_view_message"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.getViewMessage") getViewMessage

> Return the details of the message.


```php
function getViewMessage(
        $id,
        $accept)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | TODO: Add a parameter description |
| accept |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$id = 'id';
$accept = '*/*';

$result = $message->getViewMessage($id, $accept);

```


### <a name="create_send_sms_message"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.createSendSMSMessage") createSendSMSMessage

> Send a single message.


```php
function createSendSMSMessage(
        $accept,
        $senderId,
        $mobileNumber,
        $message)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| accept |  ``` Required ```  | TODO: Add a parameter description |
| senderId |  ``` Required ```  | Sender id to send the message from. |
| mobileNumber |  ``` Required ```  | The mobile number supposed to receive the message. |
| message |  ``` Required ```  | Message text. |



#### Example Usage

```php
$accept = 'Accept';
$senderId = 'senderId';
$mobileNumber = 'mobileNumber';
$message = 'message';

$result = $message->createSendSMSMessage($accept, $senderId, $mobileNumber, $message);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="sender_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SenderController") SenderController

### Get singleton instance

The singleton instance of the ``` SenderController ``` class can be accessed from the API Client.

```php
$sender = $client->getSender();
```

### <a name="get_sender_name_details"></a>![Method: ](https://apidocs.io/img/method.png ".SenderController.getSenderNameDetails") getSenderNameDetails

> Return the details of the sender name.


```php
function getSenderNameDetails(
        $id,
        $accept)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | TODO: Add a parameter description |
| accept |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$id = 'sender-id';
$accept = '*/*';

$result = $sender->getSenderNameDetails($id, $accept);

```


### <a name="create_sender_name"></a>![Method: ](https://apidocs.io/img/method.png ".SenderController.createSenderName") createSenderName

> Create a new sender id to send messages using it


```php
function createSenderName(
        $accept,
        $contentType,
        $body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| accept |  ``` Required ```  | TODO: Add a parameter description |
| contentType |  ``` Required ```  | TODO: Add a parameter description |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$accept = 'text/plain';
$contentType = 'text/plain';
$body = 'Your sender name';

$result = $sender->createSenderName($accept, $contentType, $body);

```


### <a name="get_all_senders"></a>![Method: ](https://apidocs.io/img/method.png ".SenderController.getAllSenders") getAllSenders

> List all senders names associated with the account


```php
function getAllSenders($accept)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| accept |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$accept = '*/*';

$result = $sender->getAllSenders($accept);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="balance_controller"></a>![Class: ](https://apidocs.io/img/class.png ".BalanceController") BalanceController

### Get singleton instance

The singleton instance of the ``` BalanceController ``` class can be accessed from the API Client.

```php
$balance = $client->getBalance();
```

### <a name="get_balance"></a>![Method: ](https://apidocs.io/img/method.png ".BalanceController.getBalance") getBalance

> Get your available balance


```php
function getBalance($accept)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| accept |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$accept = 'text/plain';

$result = $balance->getBalance($accept);

```


[Back to List of Controllers](#list_of_controllers)



=======
# Getting started

The Releans SDK enables developers to use Releans Services in their code. You can get started in minutes.

```composer require releans/php-client-sdk```

## Initialization

### Authentication
In order to setup authentication and initialization of the API client, you need the following information.

| Parameter | Description |
|-----------|-------------|
| oAuthAccessToken | OAuth 2.0 Access Token |



API client can be initialized as following.

```php
$oAuthAccessToken = 'oAuthAccessToken'; // OAuth 2.0 Access Token

$client = new ReleansAPILib\ReleansAPIClient($oAuthAccessToken);
```


# Class Reference

## <a name="list_of_controllers"></a>List of Controllers

* [MessageController](#message_controller)
* [SenderController](#sender_controller)
* [BalanceController](#balance_controller)

## <a name="message_controller"></a>![Class: ](https://apidocs.io/img/class.png ".MessageController") MessageController

### Get singleton instance

The singleton instance of the ``` MessageController ``` class can be accessed from the API Client.

```php
$message = $client->getMessage();
```

### <a name="get_all_messages"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.getAllMessages") getAllMessages

> List all messages sent by the account.


```php
function getAllMessages($accept)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| accept |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$accept = '*/*';

$result = $message->getAllMessages($accept);

```


### <a name="get_view_message"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.getViewMessage") getViewMessage

> Return the details of the message.


```php
function getViewMessage(
        $id,
        $accept)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | TODO: Add a parameter description |
| accept |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$id = 'id';
$accept = '*/*';

$result = $message->getViewMessage($id, $accept);

```


### <a name="create_send_sms_message"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.createSendSMSMessage") createSendSMSMessage

> Send a single message.


```php
function createSendSMSMessage(
        $accept,
        $senderId,
        $mobileNumber,
        $message)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| accept |  ``` Required ```  | TODO: Add a parameter description |
| senderId |  ``` Required ```  | Sender id to send the message from. |
| mobileNumber |  ``` Required ```  | The mobile number supposed to receive the message. |
| message |  ``` Required ```  | Message text. |



#### Example Usage

```php
$accept = 'Accept';
$senderId = 'senderId';
$mobileNumber = 'mobileNumber';
$message = 'message';

$result = $message->createSendSMSMessage($accept, $senderId, $mobileNumber, $message);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="sender_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SenderController") SenderController

### Get singleton instance

The singleton instance of the ``` SenderController ``` class can be accessed from the API Client.

```php
$sender = $client->getSender();
```

### <a name="get_sender_name_details"></a>![Method: ](https://apidocs.io/img/method.png ".SenderController.getSenderNameDetails") getSenderNameDetails

> Return the details of the sender name.


```php
function getSenderNameDetails(
        $id,
        $accept)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | TODO: Add a parameter description |
| accept |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$id = 'sender-id';
$accept = '*/*';

$result = $sender->getSenderNameDetails($id, $accept);

```


### <a name="create_sender_name"></a>![Method: ](https://apidocs.io/img/method.png ".SenderController.createSenderName") createSenderName

> Create a new sender id to send messages using it


```php
function createSenderName(
        $accept,
        $contentType,
        $body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| accept |  ``` Required ```  | TODO: Add a parameter description |
| contentType |  ``` Required ```  | TODO: Add a parameter description |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$accept = 'text/plain';
$contentType = 'text/plain';
$body = 'Your sender name';

$result = $sender->createSenderName($accept, $contentType, $body);

```


### <a name="get_all_senders"></a>![Method: ](https://apidocs.io/img/method.png ".SenderController.getAllSenders") getAllSenders

> List all senders names associated with the account


```php
function getAllSenders($accept)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| accept |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$accept = '*/*';

$result = $sender->getAllSenders($accept);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="balance_controller"></a>![Class: ](https://apidocs.io/img/class.png ".BalanceController") BalanceController

### Get singleton instance

The singleton instance of the ``` BalanceController ``` class can be accessed from the API Client.

```php
$balance = $client->getBalance();
```

### <a name="get_balance"></a>![Method: ](https://apidocs.io/img/method.png ".BalanceController.getBalance") getBalance

> Get your available balance


```php
function getBalance($accept)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| accept |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$accept = 'text/plain';

$result = $balance->getBalance($accept);

```


[Back to List of Controllers](#list_of_controllers)




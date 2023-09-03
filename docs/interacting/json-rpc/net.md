import Tabs from "@theme/Tabs";
import TabItem from "@theme/TabItem";

# Net

## net_listening


| Invocation |
| :--- |
| `{"method":"net_listening","params":[]}` |

| This method doesn't have parameters. |
| :--- |

| Returned type | Description |
| :--- | :--- |
| `Boolean` |  |

<Tabs>
<TabItem value="request" label="Request">

``` bash
curl --data '{"method":"net_listening","params":[],"id":1,"jsonrpc":"2.0"}' -H "Content-Type: application/json" -X POST localhost:8545
```
</TabItem>
<TabItem value="response" label="Response">

```yaml
{
  "jsonrpc": "2.0",
  "result": true,
  "id": 1
}
```
</TabItem>
</Tabs>

## net_localAddress

 

| Invocation |
| :--- |
| `{"method":"net_localAddress","params":[]}` |

| This method doesn't have parameters. |
| :--- |

| Returned type | Description |
| :--- | :--- |
| `Address` |  |

<Tabs>
<TabItem label="Request" value="request">

``` bash
curl --data '{"method":"net_localAddress","params":[],"id":1,"jsonrpc":"2.0"}' -H "Content-Type: application/json" -X POST localhost:8545
```
</TabItem>
<TabItem value="response" label="Response">

```yaml
{
  "jsonrpc": "2.0",
  "result": 0x247b5f5f007fb5d50de13cfcbd4460db21c12bcb,
  "id": 1
}
```
</TabItem>
</Tabs>

## net_localEnode
| Invocation |
| :--- |
| `{"method":"net_localEnode","params":[]}` |

| This method doesn't have parameters. |
| :--- |

| Returned type | Description |
| :--- | :--- |
| `String` |  |

<Tabs>
<TabItem label="Request" value="request">

``` bash
curl --data '{"method":"net_localEnode","params":[],"id":1,"jsonrpc":"2.0"}' -H "Content-Type: application/json" -X POST localhost:8545
```
</TabItem>
<TabItem value="response" label="Response">

```yaml
{
  "jsonrpc": "2.0",
  "result": enode://a9cfa3cb16b537e131b0f141b5ef0c0ab9bf0dbec7799c3fc7bf8a974ff3e74e9b3258951b285dfed07ab395049bcd65fed96116bb92561612682551ec458497@18.193.43.58:30303,
  "id": 1
}
```
</TabItem>
</Tabs>

[See also CLI net.localEnode](https://docs.nethermind.io/nethermind/nethermind-utilities/cli/net#net-localenode)
## net_peerCount
| Invocation |
| :--- |
| `{"method":"net_peerCount","params":[]}` |

| This method doesn't have parameters. |
| :--- |

| Returned type | Description |
| :--- | :--- |
| `Quantity` |  |

<Tabs>
<TabItem label="Request" value="request">

``` bash
curl --data '{"method":"net_peerCount","params":[],"id":1,"jsonrpc":"2.0"}' -H "Content-Type: application/json" -X POST localhost:8545
```
</TabItem>
<TabItem value="response" label="Response">

```yaml
{
  "jsonrpc": "2.0",
  "result": 0x11,
  "id": 1
}
```
</TabItem>
</Tabs>
[See also CLI net.peerCount](https://docs.nethermind.io/nethermind/nethermind-utilities/cli/net#net-peercount)

## net_version
| Invocation |
| :--- |
| `{"method":"net_version","params":[]}` |

| This method doesn't have parameters. |
| :--- |

| Returned type | Description |
| :--- | :--- |
| `String` |  |

<Tabs>
<TabItem label="Request" value="request">

```
curl --data '{"method":"net_version","params":[],"id":1,"jsonrpc":"2.0"}' -H "Content-Type: application/json" -X POST localhost:8545
```
</TabItem>
<TabItem value="response" label="Response">

```yaml
{
  "jsonrpc": "2.0",
  "result": 4,
  "id": 1
}
```
</TabItem>
</Tabs>
[See also CLI net.version](https://docs.nethermind.io/nethermind/nethermind-utilities/cli/net#net-version)
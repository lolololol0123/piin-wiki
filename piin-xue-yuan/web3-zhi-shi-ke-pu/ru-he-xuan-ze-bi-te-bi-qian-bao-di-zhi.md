# 🟠 如何选择比特币钱包地址

在区块链世界里，钱包地址就像“银行卡账号”一样用于接收数字资产。对于第一次接触比特币生态的朋友来说，在看到钱包里显示出的比特币地址时可能会感到疑惑：为什么钱包里有几种不同的比特币地址？这些地址有什么区别？我应该选择哪一种？



<figure><img src="../../.gitbook/assets/image (29).png" alt=""><figcaption></figcaption></figure>



所以，今天我想简单科普一下关于比特币钱包地址的相关知识，以及尝试解答一些关于不同比特币地址格式之间资产转移的常见问题。

首先为什么比特币能有这么多不同格式的地址，这些地址之间有什么区别呢？

比特币社区是一个技术不断发展的社区，每项新技术的诞生都旨在解决特定的问题，比如降低费用、增加隐私保护或提高交易速度，而不同的地址格式可以认为是新技术应用的结果。



### <mark style="color:orange;">**比特币地址类型**</mark>



* #### 第一类地址 Legacy

这类地址是在 2009 年比特币刚刚推出的时候采用的传统地址格式，所以称作 Legacy 格式，也叫普通地址，特点是都是以“1”开头。

_示例：15f12gEh2DFcHyhSyu7v3Bji5T3CJa9Smn_

因为比特币的手续费是按照交易的数据量来计价的，Legacy 类型的地址在交易中会占用更多的空间，导致交易的手续费更高。目前只会在使用一些与新地址不兼容的旧钱包时才会使用这种类型的地址。



* #### 第二类地址 Nested SegWit

在介绍之前，我们需要先对隔离见证（SegWit ）有个基本的了解，在比特币的每笔交易信息分为两个部分：基础交易数据+见证数据，前者记录账户资金结余，后者是验证用户身份。

隔离见证技术，就是将见证数据（签名信息）从交易信息中分离出来，以减小交易的数据量，进而提高交易处理的效率，降低交易成本。

因为隔离见证是兼容性升级，因此存在兼容地址和原生地址两种：

隔离见证兼容地址主要是为了兼容那些不支持隔离见证的老钱包，也就是说让那些一直没有升级的老钱包也能使用隔离见证兼容地址。

而隔离见证原生地址就不兼容老钱包了，只有支持隔离见证的钱包才能使用。

Nested SegWit 就是隔离见证兼容地址，特点是以“3”开头。

_示例：35PBEaofpUeH8VnnNSorM1QZsadrZoQp4N_

&#x20;

* #### 第三类地址 Native SegWit

这类地址就是原生隔离见证地址，特点是以 “ bc1q ” 开头。相比隔离见证兼容地址，原生隔离见证地址可以进一步减小交易体积。因此，这类地址可以享受到更低的交易费用和更快的交易速度。

_示例：bc1q42lja79elem0anu8q8s3h2n687re9jax556pcc_

&#x20;

* #### 第四类地址 Taproot

Taproot 地址，也叫主根地址，以 “ bc1p ” 开头。

Taproot 是比特币的最新升级，其结合隔离见证和其他技术优化，进一步减小了存储空间，提高了交易效率，并提供了更好的隐私性。

_示例：bc1pmzfrwwndsqmk5yh69yjr5lfgfg4ev8c0tsc06e_

&#x20;

### <mark style="color:orange;">**这四类地址该如何选择**</mark>

&#x20;

首先要明确的是，无论是哪种比特币地址，它们是由同一个私钥/助记词生成的，只要你的钱包支持，任何类型的地址都可以使用。&#x20;

目前的主流钱包比如 OKX、Unisat 等钱包都支持以上四种地址，不过为了减少交易费用，优先选择 Taproot、Native SegWit 格式的地址是比较合理的。

不过，由于 BRC20 仅支持 Taproot 地址，所以对于初次接触比特币生态的社区小伙伴们来说，直接选择 Taproot 地址格式就行。

此外，由于比特币地址是交叉兼容的，所以各类地址之间是可以相互转账的，但同时需要注意的是，不同格式的地址之间是相互隔离的，这就像同一个银行的不同的账户，每个账户里的资金都是独立的。

举个例子：如果你把资产转到 Taproot 地址里，那么在其他格式的地址中是看不到这笔资产，所以一定要清楚自己的资产存储在哪个地址里。

另一种情况，由于钱包不支持某地址格式或者某些协议，导致资产转入后不能被识别和显示出来。比如在使用 Xverse 钱包时，由于 Xverse 钱包仅支持以 “ 3 ” 开头的地址接收 BTC，以 “ bc1p ” 开头的地址接收 Ordinals 资产，如果不小心把 BTC 转移到了 Ordinals 资产接收地址，在这种情况下，Xverse 钱包是不会显示这笔 BTC 余额的。这时个时候只需要把该地址助记词导入到支持所有地址格式的钱包，然后将资产重新转移出来即可。

不过，为了避免出现此类不必要的麻烦，在钱包的选择上，建议直接使用支持全地址格式的钱包。最后，无论采用哪种地址，请务必在发送资产之前仔细检查地址信息，以防止不必要的损失。








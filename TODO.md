#TODO
- Implement the new way to genetatekey to mode `bsgs` this will improve the speed of bsgs ten times more.
- GPU support
- Make a test files for All cases of input data with fixed ranges of search
- address BTC legacy, bech32, ETH

#DONE
- Optimize Point Addition, maybe with a custom bignumber lib instead libgmp
  This was done in the version `0.1.20210412 secp256k1` we change from libgmp to secp256k1
- Added sha3 same files used by brainflayer
- Added mode rmd160
- Fixed the bug in Partition process of Introsort
- Fixed Quicksort edges cases (All data already sorted)
  To fix it Introsort was inmplement
- Fixed bottleneck of Point - Scalar multiplication
  This was fix implementing a fixed Doubling Point G
  Also part of this was made by bypassing it and implementing Point addition

#待办事项
- 实现生成密钥到“bsgs”模式的新方法，这将使 bsgs 的速度提高十倍。
- GPU 支持
- 为所有输入数据情况制作测试文件，并设置固定的搜索范围
- 地址：BTC legacy、bech32、ETH

＃完毕
- 优化点加法，或许可以使用自定义大数库（而非 libgmp）
此操作已在版本 `0.1.20210412 secp256k1` 中完成，我们将 libgmp 更改为 secp256k1
- 添加了与 brainflayer 相同的 sha3 文件
- 添加了 rmd160 模式
- 修复了 Introsort 分区过程中的错误
- 修复了快速排序边缘情况（所有数据均已排序）
为了修复此问题，我们实现了 Introsort
- 修复了点乘法的瓶颈
这是通过实现固定的倍增点 G 来实现的
此外，部分修复是通过绕过它并实现点加法来实现的

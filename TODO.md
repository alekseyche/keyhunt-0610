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

实施生成密钥模式的新方法，bsgs这将使 bsgs 的速度提高十倍。
GPU 支持
针对所有输入数据的情况，使用固定的搜索范围制作测试文件
地址 BTC legacy、bech32、ETH
＃完毕

0.1.20210412 secp256k1优化点加法，也许可以使用自定义大数库而不是 libgmp 这是在我们从 libgmp 更改为 secp256k1 的版本中完成的
添加了 brainflayer 使用的 sha3 相同文件
添加模式 rmd160
修复了 Introsort 分区过程中的 bugz
修复了 Quicksort 边缘情况（所有数据都已排序）为了修复它，Introsort 被实现
修复了点 - 标量乘法的瓶颈，这是通过实现固定的倍增点 G 来实现的，这也是通过绕过它并实现点加法来实现的

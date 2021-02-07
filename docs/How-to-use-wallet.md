# 如何使用钱包

使用venus创建钱包地址，导入和导出私钥，设置钱包密码(用来加密私钥)，锁定和解锁钱包

## 简单描述

1. 首先设置钱包密码，会用设置的密码对私钥进行加密

    ```sh
        ./venus wallet set-password <password>
    ```

2. 执行创建钱包地址、导入或导出私钥这三个操作都需要密码，所以在使用的时候确定已经设置密码，不然会导致操作执行失败

3. 重启时需要使用命令 `./venus wallet unlock <password>` 解锁钱包，不然会导致获取不到私钥，进而导致需要签名时签名失败

4. 使用 `./venus wallet lock <password>` 锁定钱包

5. 使用 `./venus wallet unlock-list` 查询已经解锁的地址

## [更多命令](Commands)
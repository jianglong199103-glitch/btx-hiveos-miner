# btx-hiveos-miner

BTX HiveOS custom miner package for `dexbtx-miner`.

## HiveOS

- Miner: `Custom`
- Custom miner name: `dexbtx`
- Installation URL: `https://raw.githubusercontent.com/jianglong199103-glitch/btx-hiveos-miner/main/dexbtx-v0.3.4-hiveos.tar.gz`
- Hash algorithm: `custom`
- Pool URL: `stratum+tcp://stratum.minebtx.com:3333`
- Password: `x`

BTX 真正的 PoW 是 `matmul`，但是 HiveOS 的 Custom miner 不靠这个下拉框启动算法，这个框只是 HiveOS 界面占位。
如果你的 HiveOS 下拉里没有 `custom`，就选 `sha256` 作为占位。

## Extra config

```text
--threads 8 --prepare-workers 16 --batch-size 128 --prefetch 8 --gpu-inputs 0 --nonces-per-slice 2000000
```

If the rig is unstable, lower it to:

```text
--threads 4 --prepare-workers 8 --batch-size 128 --prefetch 8 --gpu-inputs 0 --nonces-per-slice 2000000
```

# Rift2Core

## Rift2330

This is a simple version of [Rift2Core](https://github.com/whutddk/Rift2Core/tree/develop).
Commit: b95a1555aeb79d975e8b273d412f0e6df42d0322 (Almost...)


----------------------------

* dhrystone-500: 0.038206
* coremark: 0.112442


The configuration is as followed:
```
class Rift2330 extends Config((site, here, up) => {
  case RiftParamsKey => RiftSetting(
    hasL2  = true,
    hasDebugger = true,
    hasPreFetch = false,
    hasuBTB = false,
    ftChn = 4,
    rnChn = 2,
    opChn = 2,
    wbChn = 2,
    cm_chn = 2,
    pmpNum = 0,
    hpmNum  = 0,
    regNum = 34,
    l1BeatBits = 64,
    memBeatBits = 64,
    tlbEntry = 2,
    l1DW = 128,
    ifetchParameters = IFParameters(
      uBTB_entry = 8,
      btb_cl = 4,
      bim_cl = 8,
      ras_dp = 4,
    ),
    icacheParameters = IcacheParameters(
      cb = 1,
      cl = 2,
    ),
    dcacheParameters = DcacheParameters(
      bk = 1,
      cb = 1,
      cl = 2,
      sbEntry = 2,
      stEntry = 2,
    ),
    dptEntry = 4,
    fpuNum = 0,
    isMinArea = true,
    isLowPower = false,
  )
})
```




# iHealth Device Developer Documnentation
This document describes how to use the iHealth Device SDK to accomplish the major operation: Connection Device, Online Measurement, Offline Measurement and iHealth Device Management.

### Support iHealth Device for iOS

iHealth Bp3 
iHealth Bp5
iHealth Bp7
iHealth Bp3l
iHealth Abi
iHealth Hs3
iHealth Hs4
iHealth Hs4s
iHealth Hs5
iHealth Am3
iHealth Am3s
iHealth Am4
iHealth Po3
iHealth Bg1
iHealth Bg5

### Relevant files and frameworks
1、Import the following iHealthSDK files： BPHeader.h, BPMacroFile.h, BP3.h, BP3Controller.h, BP5.h, BP5Controller.h, BP7.h, BP7Controller.h,BP3L.h, BP3LController.h, ABI.h, ABIController.h, HSHeader.h、HSMacroFile.h、HS3.h、HS3Controller.h、HS4.h、HS4Controller.h、 HS5.h、HS5Controller.h、AMHeader.h、AMMacroFile.h、AM3.h、 AM3Controller.h、AM3S.h、AM3SController.h、User.h 、POHeader.h、POMacroFile.h、PO3.h、PO3Controller.h、iHealthLibrary.a，supports iOS 6.0 and above.

2、Frameworks


3、Configuration
Add 2 new Item in ‘Supported external accessory protocols’: com.jiuan.BPV20, com.jiuan.P930, com.jiuan.BPV21









##### 2. Operation procedure for BP5.

a) Register plug-in device info: `BP5ConnectNoti`;






a) Register plug-in device info: `BP7ConnectNoti`;







For ABI Mesure(both arm and leg)


b) Initializedcontrollerclass:

```ABIController *controller = [ABIController






b) Initializedcontrollerclass:






a) Register plug-in device info: `BP3LConnectNoti`;

b) Initialize controller classes:

```BP3LController *controller = [BP3LController
shareBP3LController];```

c) Access control class instance after receive BP3LConnectNoti: 

```NSArray *bpDeviceArray = [controller
getAllCurrentBP3LInstace];```

```BP3L *bpInstance = [bpDeviceArray objectAtIndex: i];```

d) Using ‘bpInstance’ call communication module of the device

##### 6. Operation procedure for HS3.

a) Register plug-in device HS3 info: `HS3ConnectNoti`;

b) Initialize controller class:




##### 7. Operation procedure for HS4.









a) Register plug-in device HS5 info: `HS5ConnectNoti`; 

b) Initialize HS5 controller class:

HS5Controller:





AM3Controller:

```NSArray *amDeviceArray = [controller getAllCurrentAM3Instace];```

```AM3 *amInstance = [amDeviceArray objectAtIndex:i];```







AM3SController:

```NSArray *amDeviceArray = [controller getAllCurrentAM3SInstace];```

```AM3S *amInstance = [amDeviceArray objectAtIndex:i];```







PO3Controller:

```NSArray *po3Array = [po3Controller getAllCurrentPO3Instace];```

```PO3 *po3Instance =[po3Array objectAtIndex:i]```


##### 12. Operation procedure for PO3.


PO3Controller:

```NSArray *po3Array = [po3Controller getAllCurrentPO3Instace];```

```PO3 *po3Instance =[po3Array objectAtIndex:i]```






##### 14. Operation procedure for BG5.





[Click this link]()

## Examples


[Click this link]()


[Click this link]()





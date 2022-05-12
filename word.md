
*기본적으로 배포할 때는 rest을 하는게 좋음*
> truffle migrate --reset

> truffle console 

> let lt

> Lottery.deployed().then(function(instance){lt=instance})

*테스트 할때는 경로지정 직접 해줘야함*
> truffle test test/lottery.test.js



<br>


# Ethereum 수수료
---

```
- gas(gasLimit)
- gasPrice
- ETH
- 수수료 = gas(21000) * gasPrice(1gwei == 10** 9 wei)
- 21000000000000
- 1ETH = 10 ** 18wei
```

# Gas 계산
---
```
- 32bytes 새로 저장 == 20000 gas
- 32bytes 기존 변수에 있는 값을 바꿀 때 5000gas

(기존 변수를 초기화해서 더 쓰지 않을 때 -> 10000 gas return)
```
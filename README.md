# face-datection-maixduino

## Ambiente de desenvolvimento
O maixduino oferece uma IDE própia para o desenvolvimento com suas placas, mas é possivel usar a IDE do arduino.
> [repositório para download da IDE](https://dl.sipeed.com/MAIX/MaixPy/ide/)

O uso da IDE é muito simples e descrito de forma bem explicada neste link: [documentação](https://wiki.sipeed.com/soft/maixpy/en/get_started/env_maixpyide.html)

A versão da IDE usada neste codigo foi a v0.2.5
## Drivers (necessário apenas para windows)
[Repositório para download do driver](https://dl.sipeed.com/MAIX/tools/driver)

[modo de instalação](https://wiki.sipeed.com/soft/maixpy/en/get_started/install_driver/duino.html)

## inserindo o modelo na placa
para inserir um modelo na placa foi utilizado um arquivo kfpkg que é o kmodel com um json no formato: 
```
  "version": "0.1.0",
  "files": [
    {
      "address": 0x00300000,
      "bin": "m.kmodel",
      "sha256Prefix": false
    }
  ]
}
```
que serve pra indicar em que endereço de memória será armazenado o modelo 
mais informações sobre como funciona o armazenamento e memória da placa esta disponivel nesse [link](https://wiki.sipeed.com/soft/maixpy/en/get_started/get_started_fs.html)

para inserir esse modelo na placa foi utilizado kflash_gui





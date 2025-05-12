# ESPHome configs

При необходимости выполнить компиляцию с подстановкой своих значений нужно создать файл yaml без постфикса main с необходимыми подстановками значений.

На примере файла **jxd-r6-e1eth.yaml**:
```
substitutions:
  name: "jxd-r6-e1eth"
  friendly_name: JXD-R6-E1ETH-Alex
  device_description: JXD-R6-E1ETH v1.1

packages:
  base: !include jxd-r6-e1eth-main.yaml
```
Также необходимо создать файл secrets.yaml на основе файла JXD/secrets-template.yaml с необходимыми значениями ключей и паролей

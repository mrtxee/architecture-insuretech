# flow software-architect-cource architecture-insuretech

## нагрузочное тестирование

```bash
pip freeze > requirements.txt
pip list --format=freeze > requirements.txt
#...
pip install locust
python -m pip install --upgrade pip
.venv\Scripts\Activate.ps1
#Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
python -m venv .venv

```

## установка основных компонентов
```bash

minikube status
# minikube start --vm-driver=virtualbox
# choco install virtualbox
minikube start --vm-driver=hyperv
choco install minikube
kubectl version --client

curl -LO https://dl.k8s.io/release/v1.35.0/bin/windows/amd64/kubectl.exe

```

# legend

## зона доступности -- Availability Zone, AZ
Зона доступности — логически и физически обособленный сегмент инфраструктуры внутри одного региона облачного провайдера или распределённой системы. По сути, это отдельный дата‑центр (или группа тесно связанных дата‑центров) с независимыми источниками питания, охлаждения, сетевым подключением и инженерными системами.
Ключевые характеристики
- Изоляция. Сбои в одной зоне не затрагивают другие зоны в том же регионе.
- Географическая близость. Зоны находятся в одном регионе (обычно в пределах 10–100 км), что обеспечивает низкую задержку между ними.
- Независимая инфраструктура. У каждой зоны свои:
  - энергоснабжение,
  - охлаждение,
  - сетевое оборудование,
  - каналы связи.
- Репликация данных. Данные и сервисы могут дублироваться между зонами для отказоустойчивости.
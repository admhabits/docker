Prasyart:
- Ubah Line property DNSStubListener=no
```shell
$ sudo nano /etc/systemd/resolve.conf
```
- Jalankan Container

```shell
$ docker-compose up -d
```
- Masuk kedalam container 
```shell
$ docker exec -it -u root dns-demo bash
```
- Install dnsutils packages
```shell
$ apt update && apt install dnsutils net-tools curl -y
```
- Testing Domain
```shell
$ nslookup demo.jamkrindo.id
```
```shell
$ nslookup srv-prod-1.demo.jamkrindo.id
```

```shell
$ nslookup srv-prod-2.demo.jamkrindo.id
```

```shell
$ nslookup srv-demo-2.demo.jamkrindo.id
```

```shell
$ nslookup tes.srv-demo-2.demo.jamkrindo.id
```
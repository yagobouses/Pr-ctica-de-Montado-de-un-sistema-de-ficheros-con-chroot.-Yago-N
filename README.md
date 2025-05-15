## Práctica de Montado de un sistema de ficheros con chroot

**Autor**: Yago N
</br>
---
</br>


```bash
1. Importarmos una maquina Ubunto y le metemos el disco de Kali.
```
![lsblk](/Capturas/1.png)
---
```bash
2. Iniciamos y instalamos Kali.
```
![lsblk](/capturas/2.png)


```bash
3. Ponemos el teclado en Español y iniciamos el SSh.
```
![lsblk](/capturas/3.png)


```bash
4. Nos conectamos por SSH desde PowerShell  a Kali.
```
![lsblk](/capturas/4.png)

![lsblk](/capturas/5.png)

```bash
5. Miramos archivos y particiones del Kali.
```
![lsblk](/capturas/6.png)
![lsblk](/capturas/7.png)
![lsblk](/capturas/8.png)
![lsblk](/capturas/9.png)


```bash
6. Creamos la carpeta /mnt/recuperar y la montamos en el disco SDA3.
```
![lsblk](/capturas/10.png)
![lsblk](/capturas/11.png)

```bash
7. Miramos que la información de SDA3 que contiene nuestra información de Ubuntu esta en /mnt/recuperar.
```
![lsblk](/capturas/12.png)


```bash
8. Montamos /dev en nuestra carpeta de /mnt/recuperar/dev.
```


```bash
9. Montamos /proc en nuestra carpeta de /mnt/recuperar/proc.
```


```bash
10. Montamos /sys en nuestra carpeta de /mnt/recuperar/sys.
```
![lsblk](/capturas/13.png)
```bash
11. Hacemos chroot para posicionarme donde quiero que este el directorio raíz.
```
![lsblk](/capturas/14.png)
```bash
12. Miramos el usuario de Ubuntu y compramos que este en Kali, con esto somos root en Ubuntu y le cambiamos la contraseña con passwd  usuario.
```
![lsblk](/capturas/15.png)
```bash
13. Por último, apagamos la máquina, nos cargamos el disco y comprobamos que se le ha cambiado la contraseña al usuario de Ubuntu y que podemos entrar.
```
![lsblk](/capturas/16.png)
![lsblk](/capturas/17.png)

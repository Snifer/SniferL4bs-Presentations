
# Active Directory 101
##### Snifer - *Jose Moruno Cadima*
![image](https://1.bp.blogspot.com/-VK-_9RfNk64/XDlRfOPpO_I/AAAAAAAAJw8/LGE3HEvq8dgzBEciApKD15T0ucsaHmoagCK4BGAYYCw/s1600/Sniferlabs.png|10)

---

%%htb.peru htbperu.2021  %%

- Consultor de Seguridad informática. 
###### Certificaciones: eJPT, eCPPT, OSWP, OSCP, CRTP.

- *Redes Sociales* [@SniferL4bs](https://twitter.com/sniferl4bs)

---


![[website.png|400]]![[PodcastYoutube.png|500]]

Escritor del blog 🌐 https://www.sniferl4bs.com

---
# **Disclaimer**


---
###  CONTENIDO
|                             |     |
|:--------------------------- | --- |
| 1. Active Directory         |     |
| 2. Credenciales             |     |
| 3. Usuarios Privilegiados   |     |
| 4. Kerberos                 |     |
| 5. Servicios                |     |
| 6. Hashes                   |     |
| 7. Reconocimiento de la red |     |
| 8. Verificar privilegios    |     |
|                             |     |

---

### Que es un Active Directory

![[ActiveDirectory.png]]

---

![[Pasted image 20210525162427.png]]

---
![[Pasted image 20210525162906.png]]

---
![[Pasted image 20210526011419.png]]

---


##### Lo que deseamos identificar en un dominio?

![[Pasted image 20210525163030.png]]

---

![[Pasted image 20210525163131.png]]

---

### CREDENCIALES...

📌 Usuario en dominio. 
📌 Usuario privilegiado. 
📌 Usuario de servicios.

---
### Usuarios privilegiados
![[Pasted image 20210525165343.png]]

---
![[Pasted image 20210525174928.png]]
https://risk3sixty.com/2015/02/16/administrative-accounts-in-active-directory/

---

### Servicios
💻 LDAP
💻 RDP
💻 HTTPS/HTTPS
💻 RMI
💻 SMB
💻 Kerberos

---
- **Aplicaciones configuradas conjuntamente al AD.**
- **Directorios compartidos.**
	- Información sensible
	- Credenciales, Documentación con usuarios. 

---
### Kerberos
- Kerberos fue creado por MIT. 
- Es un protocolo de autenticación, y  no autorización.
----

### Kerberos
- Microsoft realizo cambios para la implementación en AD.
- Da información de los privilegios de cada usuario, el servicio es el que define.  
---

![[Pasted image 20210528195658.png]]

---
**Ataques a Kerberos**
-   Kerberos brute-force
-   ASREPRoast
-   Kerberoasting
-   Pass the key
-   Pass the ticket
-   Silver ticket
-   Golden ticket

---

![[Pasted image 20210529123122.png]]

---
%%Creación de SPN. 

![](Pasted%20image%2020210519093916.png) %%
### Hashes
----

![[HAshesWindows.png]]

---

# Pass The Hash
---


![[Pasted image 20210528183946.png]]

---
![[Pasted image 20210528183727.png]]

---

```
reg save HKLM\sam sam
reg save HKLM\system system
```


![[Pasted image 20210528185258.png]]

---

![[Pasted image 20210528185155.png]]


---

![[Pasted image 20210528185609.png]]

--- 

**- Resolviendo una maquina de HTB**

---
**Material adicional  de referencia:**


<iframe src="https://www.youtube.com/channel/UCWzVT126IDqZHhuygkfvPaQ" width="500" height="500"></iframe>

---

[Spanish] You Do (Not) Understand Kerberos

<iframe src="https://www.youtube.com/embed/5uhk2PKkDdw" width="500" height="500"></iframe>


---
**Contacto**

- *sniferl4bs[arroba]gmail[dot]com*
- www.sniferl4bs.com
- https://t.me/HackySec



# Laboratorio de Ansible con Docker

## Objetivo

Administrar dos servidores Docker utilizando Ansible mediante un inventario y un playbook que automatiza tareas básicas de administración.

---

## Estructura del proyecto

```
ansible-lab/
├── docker-compose.yml
├── inventory.ini
├── playbook.yml
└── README.md
```

---

## Iniciar los contenedores

```bash
docker compose up -d
```

Verificar que estén ejecutándose:

```bash
docker ps
```

---

## Verificar la conexión con Ansible

```bash
ansible docker -i inventory.ini -m ping
```

---

## Ejecutar el playbook

```bash
ansible-playbook -i inventory.ini playbook.yml
```

---

## Evidencia

Agregar aquí una captura de pantalla donde se observe la ejecución exitosa del playbook.
<img width="1349" height="710" alt="prueba2" src="https://github.com/user-attachments/assets/156cadbe-4a0e-4bb0-95f7-412e19f972c5" />
<img width="1349" height="710" alt="prueba1" src="https://github.com/user-attachments/assets/7b51410e-52c2-459d-a715-0d243cbb2832" />


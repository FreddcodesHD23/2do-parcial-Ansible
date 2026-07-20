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

# Martin Bogarin - Instrucciones de Configuración

## Estado Actual
✅ Rama `martin-bogarin` está creada y lista
✅ Usuario Git configurado: Martin Bogarin <juan.bogarinjuarez@cesunbc.edu.mx>

## Requerido: Token de Acceso Personal de GitHub

GitHub ya no soporta autenticación con contraseña. Necesitas crear un Token de Acceso Personal:

### Pasos para Crear el Token:
1. Ve a: https://github.com/settings/tokens
2. Haz clic en "Generate new token" → "Generate new token (classic)"
3. Completa:
   - **Note**: "frontend2-project"
   - **Expiration**: Elige el período de tiempo apropiado
   - **Scopes**: Marca `repo` (control completo de repositorios privados)
4. Haz clic en "Generate token"
5. **Copia el token inmediatamente** (no podrás volver a verlo)

### Comandos de Configuración:
```bash
# Clona el repositorio (si no lo has hecho)
git clone https://github.com/JMBJ2457/frontend2-projet-frontend_iii.git
cd frontend2-projet-frontend_iii

# Cambia a la rama de Martin
git checkout martin-bogarin

# Configura el usuario Git
git config user.name "Martin Bogarin"
git config user.email "juan.bogarinjuarez@cesunbc.edu.mx"

# Configura el remote con el token (reemplaza TU_TOKEN con el token real)
git remote set-url origin https://JMBJ2457:TU_TOKEN@github.com/JMBJ2457/frontend2-projet-frontend_iii.git

# Sube la rama
git push --set-upstream origin martin-bogarin
```

### Alternativa: Usar Git Credential Manager
```bash
# Configura el helper de credenciales
git config --global credential.helper manager-core

# El primer push pedirá usuario y token
git push --set-upstream origin martin-bogarin
# Username: JMBJ2457
# Password: [pega tu token aquí]
```

## Listo para Trabajar
Una vez autenticado, puedes:
- Hacer cambios: `git add . && git commit -m "tu mensaje"`
- Subir cambios: `git push`
- Actualizar: `git pull`

## Información de la Rama
- **Rama**: `martin-bogarin`
- **Usuario**: JMBJ2457
- **Email**: juan.bogarinjuarez@cesunbc.edu.mx

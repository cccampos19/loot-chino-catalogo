# 🚀 Guía Completa: GitHub + Vercel Deployment

## Paso a Paso para Subir tu Catálogo Loot Chino

### PASO 1: Instalar Git (Una sola vez)

#### Windows:
1. Descarga [Git para Windows](https://git-scm.com/download/win)
2. Ejecuta el instalador
3. Usa todas las opciones por defecto (click Next)
4. Abre Command Prompt y verifica:
   ```bash
   git --version
   ```

#### Mac:
1. Abre Terminal
2. Ejecuta:
   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   brew install git
   ```

#### Linux:
```bash
sudo apt-get install git
```

---

### PASO 2: Configurar Git (Una sola vez)

```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu.email@gmail.com"
```

---

### PASO 3: Crear Repositorio en GitHub

1. Ve a [github.com](https://github.com)
2. Click en `Sign Up` (si no tienes cuenta)
3. Completa el registro
4. Click en el `+` (arriba a la derecha) → "New repository"
5. Llena:
   - **Repository name**: `loot-chino-catalogo`
   - **Description**: "Catálogo interactivo de productos chinos"
   - **Public** (así cualquiera puede verlo)
   - Click "Create repository"

6. **IMPORTANTE**: Copia la URL que aparece (algo como):
   ```
   https://github.com/TU_USUARIO/loot-chino-catalogo.git
   ```

---

### PASO 4: Subir tu Proyecto a GitHub

#### En Windows (Command Prompt):

```bash
# Navega a tu carpeta del proyecto
cd C:\Users\Carlos\Downloads\Loot cino

# Inicializa Git
git init

# Agrega todos los archivos
git add .

# Crea el primer commit
git commit -m "Initial commit: Catálogo Loot Chino con 13 productos"

# Conecta con tu repositorio (reemplaza TU_USUARIO)
git branch -M main
git remote add origin https://github.com/TU_USUARIO/loot-chino-catalogo.git

# Sube todo
git push -u origin main
```

#### En Mac/Linux:

Igual que arriba pero en Terminal.

**Resultado esperado:**
```
Enumerating objects: 15, done.
Counting objects: 100% (15/15), done.
Writing objects: 100% (15/15), ...
To https://github.com/TU_USUARIO/loot-chino-catalogo.git
 * [new branch]      main -> main
Branch 'main' set up to track remote branch 'main' from 'origin'.
```

---

### PASO 5: Verificar en GitHub

1. Ve a tu repositorio en GitHub
2. Deberías ver tus archivos:
   - ✅ `index.html`
   - ✅ `imagenes/` (carpeta con 13 imágenes)
   - ✅ `README.md`
   - ✅ `vercel.json`
   - ✅ `.gitignore`

---

### PASO 6: Crear Cuenta en Vercel

1. Ve a [vercel.com](https://vercel.com)
2. Click "Sign Up"
3. Click "Continue with GitHub"
4. Autoriza Vercel para acceder a tu GitHub
5. Completa tu perfil

---

### PASO 7: Deploy en Vercel

1. En Vercel, click "New Project"
2. En "Import Git Repository", selecciona:
   ```
   loot-chino-catalogo
   ```
3. Click "Import"
4. En "Configure Project":
   - **Framework**: "Other" (es HTML estático)
   - **Root Directory**: `./`
   - Click "Deploy"

5. **¡ESPERA A QUE TERMINE!** (2-3 minutos)

---

### PASO 8: ¡Tu Sitio Está VIVO! 🎉

Vercel te mostrará:
```
✅ Production: https://loot-chino-catalogo.vercel.app
```

**¡LISTO!** Tu catálogo está en internet.

---

## 🔄 Próximas Veces (Actualizaciones)

Cuando cambies precios o información:

```bash
# En tu carpeta del proyecto
git add .
git commit -m "Actualizar precios - septiembre 2026"
git push
```

**Vercel automáticamente redeploya en 1-2 minutos** ✅

---

## 🆘 Solución de Problemas

### ❌ "git command not found"
→ Git no está instalado. Ve a PASO 1.

### ❌ "Permission denied (publickey)"
→ Configura SSH en GitHub:
```bash
ssh-keygen -t ed25519 -C "tu.email@gmail.com"
# Sigue las instrucciones
```

### ❌ "fatal: could not read Username"
→ En Windows, usa:
```bash
git config --global credential.helper manager
```

### ❌ Las imágenes no aparecen en Vercel
→ Verifica que la carpeta sea exactamente: `imagenes/`
→ Los nombres de archivos sean exactos (mayúsculas/minúsculas importan)

### ❌ El sitio se ve mal en Vercel
→ Limpia caché del navegador: `Ctrl+Shift+Delete`

---

## 📊 Dashboard Vercel

En tu panel de Vercel podrás:

- ✅ Ver analytics de visitas
- ✅ Configurar dominio personalizado
- ✅ Ver logs de deployment
- ✅ Revertir a versiones anteriores
- ✅ Configurar HTTPS automático

---

## 🎁 Bonus: Agregar Dominio Personalizado

Si quieres `mitienda.com` en lugar de `loot-chino-catalogo.vercel.app`:

1. Compra un dominio en Namecheap, GoDaddy o Google Domains
2. En Vercel → Settings → Domains
3. Agrega tu dominio
4. Sigue las instrucciones de DNS
5. ¡Listo! En 24-48 horas estará activo

---

## ✅ Checklist Final

- [ ] Git instalado y configurado
- [ ] Repositorio creado en GitHub
- [ ] Archivos subidos a GitHub
- [ ] Cuenta de Vercel creada
- [ ] Proyecto deployeado en Vercel
- [ ] Sitio en vivo y accesible
- [ ] Imágenes visibles
- [ ] Precios correctos
- [ ] Footer con teléfono

**¡FELICIDADES!** Tu catálogo Loot Chino está en el internet 🌍

---

## 📞 Soporte Rápido

- **GitHub Help**: [docs.github.com](https://docs.github.com)
- **Vercel Docs**: [vercel.com/docs](https://vercel.com/docs)
- **Git Basics**: [git-scm.com/book](https://git-scm.com/book)

---

**Última actualización**: Septiembre 2026  
**Versión**: 1.0

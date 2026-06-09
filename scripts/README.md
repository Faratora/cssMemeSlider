# Git Commit Helper

## Как использовать

### В VS Code:

**Способ 1: Через задачу (Task)**

1. Откройте командную палитру (`Ctrl+Shift+P`)
2. Выберите `Tasks: Run Task`
3. Выберите `Generate Commit Message (Copy to Clipboard)`
4. Сообщение скопируется в буфер
5. Откройте Git панель (`Ctrl+Shift+G`) и вставьте (Ctrl+V) в поле коммита

**Способ 2: Через терминал в VS Code**

```powershell
powershell -ExecutionPolicy Bypass -File .vscode/scripts/generate-commit.ps1
```

### В любом месте (терминал):

```powershell
# Стандартное сообщение
scripts\create-commit.bat

# С кастомным префиксом
powershell -ExecutionPolicy Bypass -File scripts/create-commit.ps1 -Prefix "fix: your fix"
```

### Результат:
```
feat: add slider controls (Fri May 2026-05-29 14:24:50)
```

Формат: день недели месяц дата время (секунды)
# Guía de Archivos SVG para CupraTherm

## 📁 Estructura de Archivos

Coloca todos los archivos SVG en la carpeta `images/`:

```
images/
├── packed-bed.svg           ← Dibujo del packed bed con esferas
├── circle-main.svg          ← Círculo principal que rodea el sistema
├── copper-slag-stone.svg    ← Piedra de copper slag (ampliada)
├── arrow-connector.svg      ← Flecha que conecta esfera → piedra
├── icon-byproduct.svg       ← Ícono 1: Subproducto de pirometalurgia
├── icon-abundant.svg        ← Ícono 2: Material abundante
└── icon-thermal.svg         ← Ícono 3: Propiedades térmicas
```

## 🎨 Posicionamiento de Elementos

### Visualización del Packed Bed

El código actual usa **posicionamiento absoluto** para máxima flexibilidad:

```css
/* Cada elemento SVG tiene su propia posición */
.packed-bed-base      → z-index: 1 (fondo)
.circle-overlay       → z-index: 2 (círculo principal)
.copper-slag-stone    → z-index: 3 (piedra ampliada)
.arrow-connector      → z-index: 4 (flecha encima)
```

### Ajustar Posiciones en CSS

En `css/styles.css`, busca estas clases y modifica según necesites:

#### **Círculo Principal**
```css
.circle-overlay {
    width: 60%;           /* Tamaño del círculo */
    top: 50%;             /* Vertical (50% = centro) */
    left: 50%;            /* Horizontal (50% = centro) */
}
```

#### **Piedra de Copper Slag**
```css
.copper-slag-stone {
    width: 35%;           /* Tamaño de la piedra */
    top: 50%;             /* Ajusta arriba/abajo */
    left: 70%;            /* Ajusta izquierda/derecha */
}
```

#### **Flecha Conectora**
```css
.arrow-connector {
    width: 15%;           /* Tamaño de la flecha */
    top: 50%;             /* Ajusta vertical */
    left: 55%;            /* Ajusta horizontal */
    /* Rotar si necesitas: */
    transform: translate(-50%, -50%) rotate(45deg);
}
```

## 📐 Ejemplos de Ajustes Comunes

### Mover la piedra más arriba y a la derecha:
```css
.copper-slag-stone {
    top: 35%;    /* Más arriba (menor %) */
    left: 80%;   /* Más a la derecha (mayor %) */
}
```

### Hacer el círculo más grande:
```css
.circle-overlay {
    width: 75%;  /* Era 60%, ahora más grande */
}
```

### Rotar la flecha 30 grados:
```css
.arrow-connector {
    transform: translate(-50%, -50%) rotate(30deg);
}
```

## 🔧 Tips Importantes

1. **Mantener archivos separados**: Es más fácil editar en Illustrator/Inkscape
2. **Exportar SVG optimizado**: Usa "Save for Web" o SVGO
3. **Viewbox correcto**: Asegúrate que cada SVG tenga su viewBox definido
4. **Colores consistentes**: Usa las variables CSS del proyecto:
   - `#b87333` (copper primary)
   - `#8b5a2b` (copper dark)
   - `#e74c3c` (thermal red)

## 🎯 Workflow Recomendado

1. **Crear/editar SVG** en tu editor gráfico favorito
2. **Guardar en `images/`** con el nombre correcto
3. **Recargar el navegador** para ver cambios
4. **Ajustar posición/tamaño en CSS** si es necesario
5. **Repetir** hasta que esté perfecto

## 📱 Responsive

Los tamaños se ajustan automáticamente en móviles:
- En tablets/móviles, la piedra se hace un poco más grande (45%)
- La flecha se ajusta (20%)
- Todo mantiene proporciones

## ❓ ¿Combinar SVGs o Mantenerlos Separados?

✅ **MANTENER SEPARADOS (recomendado)**
- Mayor flexibilidad de posicionamiento
- Fácil editar individualmente
- Mejor para animaciones futuras
- Más mantenible

❌ **Combinar en un solo SVG**
- Menos flexible
- Más difícil ajustar posiciones
- Requiere editar el SVG completo cada vez

## 🚀 Siguiente Paso

1. Coloca tus 7 archivos SVG en la carpeta `images/`
2. Abre `index.html` en el navegador
3. Ajusta posiciones en `styles.css` según tu diseño
4. ¡Disfruta! 🎉

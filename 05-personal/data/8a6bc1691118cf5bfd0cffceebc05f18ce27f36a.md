# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: test\05_registrar_empleado.spec.ts >> Registrar Empleado >> Fecha de creación debe mostrarse en formato DD/MM/YYYY
- Location: e2e\test\05_registrar_empleado.spec.ts:277:9

# Error details

```
Error: expect(received).toMatch(expected)

Expected pattern: /^\d{2}\/\d{2}\/\d{4}$/
Received string:  "09 17:23:49.907478/05/2026"
```

# Page snapshot

```yaml
- generic [ref=e1]:
  - button "Cambiar tema" [ref=e3] [cursor=pointer]:
    - img [ref=e4]
  - generic [ref=e6]:
    - complementary [ref=e8]:
      - img "Migraciones Logo" [ref=e12]
      - button "Maria Lopez SUPERVISOR" [ref=e14] [cursor=pointer]:
        - img [ref=e17]
        - generic [ref=e20]:
          - paragraph [ref=e21]: Maria Lopez
          - paragraph [ref=e22]: SUPERVISOR
      - navigation [ref=e23]:
        - link "Inicio" [ref=e24] [cursor=pointer]:
          - /url: /dashboard
          - img [ref=e25]
          - paragraph [ref=e27]: Inicio
        - link "Cambios" [ref=e28] [cursor=pointer]:
          - /url: /dashboard/cambios
          - img [ref=e29]
          - paragraph [ref=e31]: Cambios
        - link "Licencias" [ref=e32] [cursor=pointer]:
          - /url: /dashboard/licencias
          - img [ref=e33]
          - paragraph [ref=e35]: Licencias
        - link "Calificaciones" [ref=e36] [cursor=pointer]:
          - /url: /dashboard/calificaciones
          - img [ref=e37]
          - paragraph [ref=e39]: Calificaciones
        - link "Personal" [ref=e40] [cursor=pointer]:
          - /url: /dashboard/personal
          - img [ref=e41]
          - paragraph [ref=e43]: Personal
        - link "Faltas" [ref=e44] [cursor=pointer]:
          - /url: /dashboard/faltas
          - img [ref=e45]
          - paragraph [ref=e47]: Faltas
        - link "Sanciones" [ref=e48] [cursor=pointer]:
          - /url: /dashboard/sanciones
          - img [ref=e49]
          - paragraph [ref=e51]: Sanciones
      - button "Cerrar Sesión" [ref=e53] [cursor=pointer]:
        - img [ref=e54]
        - generic [ref=e57]: Cerrar Sesión
    - generic [ref=e58]:
      - generic [ref=e60]:
        - generic [ref=e61]:
          - heading "Gestión de Empleados" [level=1] [ref=e62]
          - paragraph [ref=e63]: Administra los empleados, turnos y permisos del sistema WorkShift
        - button "Exportar Datos" [ref=e66] [cursor=pointer]:
          - img [ref=e67]
          - text: Exportar Datos
        - generic [ref=e70]:
          - generic [ref=e72]:
            - generic [ref=e73]:
              - paragraph [ref=e74]: Total Empleados
              - paragraph [ref=e75]: "37"
            - img [ref=e77]
          - generic [ref=e81]:
            - generic [ref=e82]:
              - paragraph [ref=e83]: Activos
              - paragraph [ref=e84]: "37"
            - img [ref=e86]
          - generic [ref=e89]:
            - generic [ref=e90]:
              - paragraph [ref=e91]: En Licencia
              - paragraph [ref=e92]: "0"
            - img [ref=e94]
          - generic [ref=e97]:
            - generic [ref=e98]:
              - paragraph [ref=e99]: Inactivo/Bloqueado
              - paragraph [ref=e100]: "0"
            - img [ref=e102]
        - generic [ref=e104]:
          - generic [ref=e106]:
            - img [ref=e107]
            - textbox "Buscar por nombre, email o Legajo..." [ref=e110]
          - generic [ref=e111]:
            - combobox [ref=e112]:
              - option "Todos los Roles" [selected]
              - option "Jefe"
              - option "Supervisor"
              - option "Inspector"
            - combobox [ref=e113]:
              - option "Todos los Turnos" [selected]
              - option "Turno A"
              - option "Turno B"
            - combobox [disabled] [ref=e114]:
              - option "Seleccionar horario laboral" [selected]
            - button "Nuevo Empleado" [ref=e115] [cursor=pointer]:
              - img [ref=e116]
              - text: Nuevo Empleado
        - generic [ref=e120]:
          - generic [ref=e121]:
            - generic [ref=e122]: "Mostrar:"
            - combobox [ref=e123]:
              - option "5"
              - option "10" [selected]
              - option "20"
              - option "50"
            - generic [ref=e124]: empleados por página
          - generic [ref=e125]: Mostrando 1 a 10 de 37 empleados
          - generic [ref=e126]:
            - button "Primera" [disabled] [ref=e127]
            - button "Anterior" [disabled] [ref=e128]
            - generic [ref=e129]: Página 1 de 4
            - button "Siguiente" [ref=e130] [cursor=pointer]
            - button "Última" [ref=e131] [cursor=pointer]
        - table [ref=e134]:
          - rowgroup [ref=e135]:
            - row "Empleado Rol Turno Horario Estado Acciones" [ref=e136]:
              - columnheader "Empleado" [ref=e137]
              - columnheader "Rol" [ref=e138]
              - columnheader "Turno" [ref=e139]
              - columnheader "Horario" [ref=e140]
              - columnheader "Estado" [ref=e141]
              - columnheader "Acciones" [ref=e142]
          - rowgroup [ref=e143]:
            - 'row "JG Juan Garcia juan.garcia@workshift.com Legajo: 300006 INSPECTOR B 14:00-23:00 ACTIVO" [ref=e144]':
              - 'cell "JG Juan Garcia juan.garcia@workshift.com Legajo: 300006" [ref=e145]':
                - generic [ref=e146]:
                  - generic [ref=e148]: JG
                  - generic [ref=e149]:
                    - generic [ref=e150]: Juan Garcia
                    - generic [ref=e151]: juan.garcia@workshift.com
                    - generic [ref=e152]: "Legajo: 300006"
              - cell "INSPECTOR" [ref=e153]:
                - generic [ref=e154]: INSPECTOR
              - cell "B" [ref=e155]:
                - generic [ref=e156]: B
              - cell "14:00-23:00" [ref=e157]
              - cell "ACTIVO" [ref=e158]:
                - generic [ref=e159]: ACTIVO
              - cell [ref=e160]:
                - generic [ref=e161]:
                  - button "Ver detalles" [active] [ref=e162] [cursor=pointer]:
                    - img [ref=e163]
                  - button "Editar" [ref=e166] [cursor=pointer]:
                    - img [ref=e167]
                  - button "Eliminar" [ref=e169] [cursor=pointer]:
                    - img [ref=e170]
            - 'row "AG Ana García ana.garcia.42133@wsms.com Legajo: 42133 INSPECTOR A 04:00-14:00 ACTIVO" [ref=e173]':
              - 'cell "AG Ana García ana.garcia.42133@wsms.com Legajo: 42133" [ref=e174]':
                - generic [ref=e175]:
                  - generic [ref=e177]: AG
                  - generic [ref=e178]:
                    - generic [ref=e179]: Ana García
                    - generic [ref=e180]: ana.garcia.42133@wsms.com
                    - generic [ref=e181]: "Legajo: 42133"
              - cell "INSPECTOR" [ref=e182]:
                - generic [ref=e183]: INSPECTOR
              - cell "A" [ref=e184]:
                - generic [ref=e185]: A
              - cell "04:00-14:00" [ref=e186]
              - cell "ACTIVO" [ref=e187]:
                - generic [ref=e188]: ACTIVO
              - cell [ref=e189]:
                - generic [ref=e190]:
                  - button "Ver detalles" [ref=e191] [cursor=pointer]:
                    - img [ref=e192]
                  - button "Editar" [ref=e195] [cursor=pointer]:
                    - img [ref=e196]
                  - button "Eliminar" [ref=e198] [cursor=pointer]:
                    - img [ref=e199]
            - 'row "AG Ana García ana.garcia.47376@wsms.com Legajo: 47376 INSPECTOR A 04:00-14:00 ACTIVO" [ref=e202]':
              - 'cell "AG Ana García ana.garcia.47376@wsms.com Legajo: 47376" [ref=e203]':
                - generic [ref=e204]:
                  - generic [ref=e206]: AG
                  - generic [ref=e207]:
                    - generic [ref=e208]: Ana García
                    - generic [ref=e209]: ana.garcia.47376@wsms.com
                    - generic [ref=e210]: "Legajo: 47376"
              - cell "INSPECTOR" [ref=e211]:
                - generic [ref=e212]: INSPECTOR
              - cell "A" [ref=e213]:
                - generic [ref=e214]: A
              - cell "04:00-14:00" [ref=e215]
              - cell "ACTIVO" [ref=e216]:
                - generic [ref=e217]: ACTIVO
              - cell [ref=e218]:
                - generic [ref=e219]:
                  - button "Ver detalles" [ref=e220] [cursor=pointer]:
                    - img [ref=e221]
                  - button "Editar" [ref=e224] [cursor=pointer]:
                    - img [ref=e225]
                  - button "Eliminar" [ref=e227] [cursor=pointer]:
                    - img [ref=e228]
            - 'row "AG Ana García emailunico.82665@wsms.com Legajo: 82665 INSPECTOR A 04:00-14:00 ACTIVO" [ref=e231]':
              - 'cell "AG Ana García emailunico.82665@wsms.com Legajo: 82665" [ref=e232]':
                - generic [ref=e233]:
                  - generic [ref=e235]: AG
                  - generic [ref=e236]:
                    - generic [ref=e237]: Ana García
                    - generic [ref=e238]: emailunico.82665@wsms.com
                    - generic [ref=e239]: "Legajo: 82665"
              - cell "INSPECTOR" [ref=e240]:
                - generic [ref=e241]: INSPECTOR
              - cell "A" [ref=e242]:
                - generic [ref=e243]: A
              - cell "04:00-14:00" [ref=e244]
              - cell "ACTIVO" [ref=e245]:
                - generic [ref=e246]: ACTIVO
              - cell [ref=e247]:
                - generic [ref=e248]:
                  - button "Ver detalles" [ref=e249] [cursor=pointer]:
                    - img [ref=e250]
                  - button "Editar" [ref=e253] [cursor=pointer]:
                    - img [ref=e254]
                  - button "Eliminar" [ref=e256] [cursor=pointer]:
                    - img [ref=e257]
            - 'row "AG Ana García legajounico.44314@wsms.com Legajo: 44314 INSPECTOR A 04:00-14:00 ACTIVO" [ref=e260]':
              - 'cell "AG Ana García legajounico.44314@wsms.com Legajo: 44314" [ref=e261]':
                - generic [ref=e262]:
                  - generic [ref=e264]: AG
                  - generic [ref=e265]:
                    - generic [ref=e266]: Ana García
                    - generic [ref=e267]: legajounico.44314@wsms.com
                    - generic [ref=e268]: "Legajo: 44314"
              - cell "INSPECTOR" [ref=e269]:
                - generic [ref=e270]: INSPECTOR
              - cell "A" [ref=e271]:
                - generic [ref=e272]: A
              - cell "04:00-14:00" [ref=e273]
              - cell "ACTIVO" [ref=e274]:
                - generic [ref=e275]: ACTIVO
              - cell [ref=e276]:
                - generic [ref=e277]:
                  - button "Ver detalles" [ref=e278] [cursor=pointer]:
                    - img [ref=e279]
                  - button "Editar" [ref=e282] [cursor=pointer]:
                    - img [ref=e283]
                  - button "Eliminar" [ref=e285] [cursor=pointer]:
                    - img [ref=e286]
            - 'row "AG Ana García ana.garcia.49813@wsms.com Legajo: 49813 INSPECTOR A 04:00-14:00 ACTIVO" [ref=e289]':
              - 'cell "AG Ana García ana.garcia.49813@wsms.com Legajo: 49813" [ref=e290]':
                - generic [ref=e291]:
                  - generic [ref=e293]: AG
                  - generic [ref=e294]:
                    - generic [ref=e295]: Ana García
                    - generic [ref=e296]: ana.garcia.49813@wsms.com
                    - generic [ref=e297]: "Legajo: 49813"
              - cell "INSPECTOR" [ref=e298]:
                - generic [ref=e299]: INSPECTOR
              - cell "A" [ref=e300]:
                - generic [ref=e301]: A
              - cell "04:00-14:00" [ref=e302]
              - cell "ACTIVO" [ref=e303]:
                - generic [ref=e304]: ACTIVO
              - cell [ref=e305]:
                - generic [ref=e306]:
                  - button "Ver detalles" [ref=e307] [cursor=pointer]:
                    - img [ref=e308]
                  - button "Editar" [ref=e311] [cursor=pointer]:
                    - img [ref=e312]
                  - button "Eliminar" [ref=e314] [cursor=pointer]:
                    - img [ref=e315]
            - 'row "AG Ana García emailunico.86098@wsms.com Legajo: 86098 INSPECTOR A 04:00-14:00 ACTIVO" [ref=e318]':
              - 'cell "AG Ana García emailunico.86098@wsms.com Legajo: 86098" [ref=e319]':
                - generic [ref=e320]:
                  - generic [ref=e322]: AG
                  - generic [ref=e323]:
                    - generic [ref=e324]: Ana García
                    - generic [ref=e325]: emailunico.86098@wsms.com
                    - generic [ref=e326]: "Legajo: 86098"
              - cell "INSPECTOR" [ref=e327]:
                - generic [ref=e328]: INSPECTOR
              - cell "A" [ref=e329]:
                - generic [ref=e330]: A
              - cell "04:00-14:00" [ref=e331]
              - cell "ACTIVO" [ref=e332]:
                - generic [ref=e333]: ACTIVO
              - cell [ref=e334]:
                - generic [ref=e335]:
                  - button "Ver detalles" [ref=e336] [cursor=pointer]:
                    - img [ref=e337]
                  - button "Editar" [ref=e340] [cursor=pointer]:
                    - img [ref=e341]
                  - button "Eliminar" [ref=e343] [cursor=pointer]:
                    - img [ref=e344]
            - 'row "AG Ana García legajounico.70023@wsms.com Legajo: 70023 INSPECTOR A 04:00-14:00 ACTIVO" [ref=e347]':
              - 'cell "AG Ana García legajounico.70023@wsms.com Legajo: 70023" [ref=e348]':
                - generic [ref=e349]:
                  - generic [ref=e351]: AG
                  - generic [ref=e352]:
                    - generic [ref=e353]: Ana García
                    - generic [ref=e354]: legajounico.70023@wsms.com
                    - generic [ref=e355]: "Legajo: 70023"
              - cell "INSPECTOR" [ref=e356]:
                - generic [ref=e357]: INSPECTOR
              - cell "A" [ref=e358]:
                - generic [ref=e359]: A
              - cell "04:00-14:00" [ref=e360]
              - cell "ACTIVO" [ref=e361]:
                - generic [ref=e362]: ACTIVO
              - cell [ref=e363]:
                - generic [ref=e364]:
                  - button "Ver detalles" [ref=e365] [cursor=pointer]:
                    - img [ref=e366]
                  - button "Editar" [ref=e369] [cursor=pointer]:
                    - img [ref=e370]
                  - button "Eliminar" [ref=e372] [cursor=pointer]:
                    - img [ref=e373]
            - 'row "AG Ana García emailunico.21077@wsms.com Legajo: 21077 INSPECTOR A 04:00-14:00 ACTIVO" [ref=e376]':
              - 'cell "AG Ana García emailunico.21077@wsms.com Legajo: 21077" [ref=e377]':
                - generic [ref=e378]:
                  - generic [ref=e380]: AG
                  - generic [ref=e381]:
                    - generic [ref=e382]: Ana García
                    - generic [ref=e383]: emailunico.21077@wsms.com
                    - generic [ref=e384]: "Legajo: 21077"
              - cell "INSPECTOR" [ref=e385]:
                - generic [ref=e386]: INSPECTOR
              - cell "A" [ref=e387]:
                - generic [ref=e388]: A
              - cell "04:00-14:00" [ref=e389]
              - cell "ACTIVO" [ref=e390]:
                - generic [ref=e391]: ACTIVO
              - cell [ref=e392]:
                - generic [ref=e393]:
                  - button "Ver detalles" [ref=e394] [cursor=pointer]:
                    - img [ref=e395]
                  - button "Editar" [ref=e398] [cursor=pointer]:
                    - img [ref=e399]
                  - button "Eliminar" [ref=e401] [cursor=pointer]:
                    - img [ref=e402]
            - 'row "AG Ana García legajounico.78840@wsms.com Legajo: 78840 INSPECTOR A 04:00-14:00 ACTIVO" [ref=e405]':
              - 'cell "AG Ana García legajounico.78840@wsms.com Legajo: 78840" [ref=e406]':
                - generic [ref=e407]:
                  - generic [ref=e409]: AG
                  - generic [ref=e410]:
                    - generic [ref=e411]: Ana García
                    - generic [ref=e412]: legajounico.78840@wsms.com
                    - generic [ref=e413]: "Legajo: 78840"
              - cell "INSPECTOR" [ref=e414]:
                - generic [ref=e415]: INSPECTOR
              - cell "A" [ref=e416]:
                - generic [ref=e417]: A
              - cell "04:00-14:00" [ref=e418]
              - cell "ACTIVO" [ref=e419]:
                - generic [ref=e420]: ACTIVO
              - cell [ref=e421]:
                - generic [ref=e422]:
                  - button "Ver detalles" [ref=e423] [cursor=pointer]:
                    - img [ref=e424]
                  - button "Editar" [ref=e427] [cursor=pointer]:
                    - img [ref=e428]
                  - button "Eliminar" [ref=e430] [cursor=pointer]:
                    - img [ref=e431]
        - generic [ref=e435]:
          - generic [ref=e437]:
            - heading "Detalles del Empleado" [level=2] [ref=e438]
            - button "Cerrar modal" [ref=e439] [cursor=pointer]:
              - img [ref=e440]
          - generic [ref=e444]:
            - generic [ref=e445]:
              - generic [ref=e446]:
                - paragraph [ref=e447]: Cuenta creada
                - paragraph [ref=e448]: 09 17:23:49.907478/05/2026
              - generic [ref=e449]:
                - paragraph [ref=e450]: Legajo
                - paragraph [ref=e451]: "300006"
              - generic [ref=e452]:
                - paragraph [ref=e453]: Estado
                - generic [ref=e454]: ACTIVO
            - generic [ref=e455]:
              - generic [ref=e456]:
                - paragraph [ref=e457]: Nombre Completo
                - paragraph [ref=e458]: Juan Garcia
              - generic [ref=e459]:
                - paragraph [ref=e460]: Email
                - paragraph [ref=e461]: juan.garcia@workshift.com
            - generic [ref=e462]:
              - generic [ref=e463]:
                - paragraph [ref=e464]: Rol
                - generic [ref=e465]: INSPECTOR
              - generic [ref=e466]:
                - paragraph [ref=e467]: Grupo de Turno
                - generic [ref=e468]: B
            - generic [ref=e469]:
              - generic [ref=e470]:
                - paragraph [ref=e471]: Horario Laboral
                - paragraph [ref=e472]: 14:00-23:00
              - generic [ref=e473]:
                - paragraph [ref=e474]: Teléfono
                - paragraph [ref=e475]: No registrado
            - generic [ref=e476]:
              - generic [ref=e477]:
                - paragraph [ref=e478]: Fecha de Nacimiento
                - paragraph
              - generic [ref=e479]:
                - paragraph [ref=e480]: Última actualización
                - paragraph [ref=e481]: 9 may 2026
            - generic [ref=e482]:
              - paragraph [ref=e483]: Dirección
              - paragraph [ref=e484]: No registrada
            - generic [ref=e485]:
              - heading "Estadísticas del Mes" [level=3] [ref=e486]
              - generic [ref=e487]:
                - generic [ref=e488]:
                  - paragraph [ref=e489]: Turnos
                  - paragraph [ref=e490]: "0"
                - generic [ref=e491]:
                  - paragraph [ref=e492]: Horas
                  - paragraph [ref=e493]: "0"
                - generic [ref=e494]:
                  - paragraph [ref=e495]: Intercambios
                  - paragraph [ref=e496]: "0"
          - button "Cancelar" [ref=e498] [cursor=pointer]
      - contentinfo [ref=e499]:
        - generic [ref=e500]: © 2026 Gestión de Turnos. Todos los derechos reservados.
        - generic [ref=e501]:
          - link "Política de Privacidad" [ref=e502] [cursor=pointer]:
            - /url: /dashboard/privacy
          - generic [ref=e503]: "|"
          - link "Términos y Condiciones" [ref=e504] [cursor=pointer]:
            - /url: /dashboard/terms
        - generic [ref=e505]:
          - generic [ref=e506]: Powered by
          - img "WSMS Logo" [ref=e508]
    - button [ref=e509] [cursor=pointer]:
      - img [ref=e510]
    - button "Abrir asistente" [ref=e512] [cursor=pointer]:
      - img [ref=e513]
  - button "Open Next.js Dev Tools" [ref=e520] [cursor=pointer]:
    - img [ref=e521]
  - alert [ref=e524]
```

# Test source

```ts
  203 |         });
  204 | 
  205 |         await test.step('Verificar mensaje de error de fecha futura', async () => {
  206 |             await expect(page.getByText('La fecha de nacimiento no puede ser futura')).toBeVisible({ timeout: 3000 });
  207 |         });
  208 |     });
  209 | 
  210 |     test('Empleado menor de 18 años muestra error', async ({ page }) => {
  211 |         await test.step('Abrir el formulario e ingresar fecha de nacimiento de menor de edad (01/01/2009)', async () => {
  212 |             await abrirFormularioCrear(page);
  213 |             await completarObligatorios(page, { legajo: uid() });
  214 |             await page.locator('form').locator('input[type="date"]').first().fill('2009-01-01');
  215 |         });
  216 | 
  217 |         await test.step('Enviar el formulario', async () => {
  218 |             await page.locator('button:has-text("Crear Empleado")').click();
  219 |             await scrollModalAlTop(page);
  220 |         });
  221 | 
  222 |         await test.step('Verificar mensaje de error de edad mínima requerida', async () => {
  223 |             await expect(page.getByText('Debes ser mayor de 18 años')).toBeVisible({ timeout: 3000 });
  224 |         });
  225 |     });
  226 | 
  227 |     // ── Bugs conocidos ────────────────────────────────────────────
  228 | 
  229 |     test('Legajo negativo debe mostrar error', {
  230 |         annotation: [
  231 |             { type: 'Severidad', description: 'Alta' },
  232 |             { type: 'Prioridad', description: 'Alta' },
  233 |             { type: 'Descripción del bug', description: 'El sistema acepta legajos negativos sin mostrar error. Un número negativo no es un identificador válido y podría provocar inconsistencias en la base de datos.' },
  234 |         ],
  235 |     }, async ({ page }) => {
  236 |         await test.step('Abrir el formulario e ingresar legajo negativo (-5)', async () => {
  237 |             await abrirFormularioCrear(page);
  238 |             await completarObligatorios(page, { legajo: '-5', email: `bug01.${uid()}@wsms.com` });
  239 |         });
  240 | 
  241 |         await test.step('Enviar el formulario', async () => {
  242 |             await page.locator('button:has-text("Crear Empleado")').click();
  243 |             await scrollModalAlTop(page);
  244 |         });
  245 | 
  246 |         await test.step('Verificar que el sistema rechaza el legajo negativo', async () => {
  247 |             await expect(
  248 |                 page.getByText('El legajo debe ser un número entero positivo')
  249 |             ).toBeVisible({ timeout: 3000 });
  250 |         });
  251 |     });
  252 | 
  253 |     test('Nombre con más de 50 caracteres debe mostrar error', {
  254 |         annotation: [
  255 |             { type: 'Severidad', description: 'Media' },
  256 |             { type: 'Prioridad', description: 'Media' },
  257 |             { type: 'Descripción del bug', description: 'El sistema acepta nombres y apellidos de más de 50 caracteres sin validar. La base de datos tiene un límite de 50 caracteres, lo que puede provocar un error al intentar guardar el registro.' },
  258 |         ],
  259 |     }, async ({ page }) => {
  260 |         const nombreLargo = 'Mariadelcarmenisabelcristinaalejandravalentinaxyz'; // 51 chars
  261 | 
  262 |         await test.step('Abrir el formulario e ingresar nombre de 51 caracteres', async () => {
  263 |             await abrirFormularioCrear(page);
  264 |             await completarObligatorios(page, { nombre: nombreLargo, legajo: uid(), email: `bug02.${uid()}@wsms.com` });
  265 |         });
  266 | 
  267 |         await test.step('Enviar el formulario', async () => {
  268 |             await page.locator('button:has-text("Crear Empleado")').click();
  269 |             await scrollModalAlTop(page);
  270 |         });
  271 | 
  272 |         await test.step('Verificar que el sistema rechaza nombres que superan los 50 caracteres', async () => {
  273 |             await expect(page.getByText(/50 caracteres/)).toBeVisible({ timeout: 3000 });
  274 |         });
  275 |     });
  276 | 
  277 |     test('Fecha de creación debe mostrarse en formato DD/MM/YYYY', {
  278 |         annotation: [
  279 |             { type: 'Severidad', description: 'Baja' },
  280 |             { type: 'Prioridad', description: 'Baja' },
  281 |             { type: 'Descripción del bug', description: 'El campo "Cuenta creada" muestra el timestamp completo del servidor en lugar de la fecha formateada. Por ejemplo: "27 20:08:22.359847/05/2026" en vez de "27/05/2026".' },
  282 |         ],
  283 |     }, async ({ page }) => {
  284 |         await test.step('Abrir el detalle del primer empleado', async () => {
  285 |             await page.locator('button[title="Ver detalles"]').first().click();
  286 |             await expect(page.getByText('Cuenta creada')).toBeVisible({ timeout: 3000 });
  287 |         });
  288 | 
  289 |         await test.step('Leer el valor del campo "Cuenta creada"', async () => {
  290 |             const fechaText = await page.evaluate(() => {
  291 |                 const labels = document.querySelectorAll('p');
  292 |                 for (const label of labels) {
  293 |                     if (label.textContent?.trim() === 'Cuenta creada') {
  294 |                         const parent = label.closest('div');
  295 |                         const valueEl = parent?.querySelectorAll('p')[1];
  296 |                         return valueEl?.textContent?.trim() ?? '';
  297 |                     }
  298 |                 }
  299 |                 return '';
  300 |             });
  301 | 
  302 |             await test.step('Verificar que el formato es DD/MM/YYYY', async () => {
> 303 |                 expect(fechaText).toMatch(/^\d{2}\/\d{2}\/\d{4}$/);
      |                                   ^ Error: expect(received).toMatch(expected)
  304 |             });
  305 |         });
  306 |     });
  307 | });
  308 | 
```
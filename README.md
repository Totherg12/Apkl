# N1K Face Overlay

Projeto Android experimental: captura a tela com MediaProjection, executa detecção facial
do ML Kit e desenha caixas/marcadores em uma camada flutuante.

## Limitações
- Não é aimbot: não toca na tela, não move a mira e não interage com o Free Fire.
- O detector foi feito para rostos em imagens comuns. Modelos/personagens 3D de jogos
  podem não ser reconhecidos ou podem gerar falsos positivos.
- O primeiro uso exige autorização de captura de tela e permissão de sobreposição.
- O Android mostra um indicador/notificação de captura enquanto o serviço está ativo.

## Abrir e compilar
Abra a pasta no Android Studio com JDK 17 e Android SDK 35.
Depois execute:

```bash
./gradlew assembleDebug
```

O APK, se a compilação for bem-sucedida, ficará em
`app/build/outputs/apk/debug/app-debug.apk`.

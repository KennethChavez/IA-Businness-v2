# Configuración Google OAuth para IA-Business

## URLs de redirección autorizadas (Google Console):

### Para desarrollo:
- http://localhost:5173
- http://localhost:5174
- http://localhost:3000

### Para producción:
- https://pqoijezzmstqgmgnnikl.supabase.co/auth/v1/callback

## Configuración en Supabase:

1. Ve a: Authentication → Providers
2. Habilita Google Provider
3. Configura:
   - **Client ID**: 748786845706-ook857oki7fdkl8jgdh0m884v2193g4k.apps.googleusercontent.com
   - **Client Secret**: [Obtener de Google Console]
   - **Redirect URL**: https://pqoijezzmstqgmgnnikl.supabase.co/auth/v1/callback

## Para probar el login:

1. Asegúrate de que el servidor de desarrollo esté corriendo
2. Haz clic en "Comenzar con Google" en la página principal
3. Deberías ser redirigido a Google para autenticarte
4. Después del login exitoso, serás redirigido al dashboard

## Troubleshooting:

Si tienes problemas:
- Verifica que las URLs de redirección coincidan exactamente
- Asegúrate de que Google+ API esté habilitada en Google Console
- Revisa la consola del navegador para errores
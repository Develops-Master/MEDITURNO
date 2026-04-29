# MEDITURNO
MEDITURNO - SISTEMA COMPLETO CON API  -  ASP NET CORE MVC .NET 10  -  LUIS MANCO BERROCAL
MediTurno/
│
├── MediTurno.sln
│
├── src/
│   ├── MediTurno.Core/                           # NÚCLEO - Entidades e Interfaces
│   │   ├── Entities/
│   │   │   ├── Base/
│   │   │   │   ├── BaseEntity.cs
│   │   │   │   ├── IAuditableEntity.cs
│   │   │   │   └── ISoftDelete.cs
│   │   │   ├── Usuario.cs
│   │   │   ├── Rol.cs
│   │   │   ├── Permiso.cs
│   │   │   ├── RolPermiso.cs
│   │   │   ├── Paciente.cs
│   │   │   ├── Medico.cs
│   │   │   ├── Secretaria.cs
│   │   │   ├── Especialidad.cs
│   │   │   ├── SubEspecialidad.cs
│   │   │   ├── HorarioMedico.cs
│   │   │   ├── Cita.cs
│   │   │   ├── HistorialClinico.cs
│   │   │   ├── Diagnostico.cs
│   │   │   ├── RecetaMedica.cs
│   │   │   ├── DetalleReceta.cs
│   │   │   ├── Medicamento.cs
│   │   │   ├── CategoriaMedicamento.cs
│   │   │   ├── Inventario.cs
│   │   │   ├── MovimientoInventario.cs
│   │   │   ├── Producto.cs
│   │   │   ├── CategoriaProducto.cs
│   │   │   ├── Factura.cs
│   │   │   ├── DetalleFactura.cs
│   │   │   ├── Pago.cs
│   │   │   ├── MetodoPago.cs
│   │   │   ├── TransaccionPago.cs
│   │   │   ├── ComprobanteElectronico.cs
│   │   │   ├── Notificacion.cs
│   │   │   ├── LogActividad.cs
│   │   │   ├── Configuracion.cs
│   │   │   ├── DocumentoAdjunto.cs
│   │   │   ├── Teleconsulta.cs
│   │   │   ├── Cama.cs
│   │   │   ├── Hospitalizacion.cs
│   │   │   ├── Quirofano.cs
│   │   │   ├── Cirugia.cs
│   │   │   ├── Laboratorio.cs
│   │   │   ├── ExamenLaboratorio.cs
│   │   │   ├── OrdenExamen.cs
│   │   │   ├── ResultadoExamen.cs
│   │   │   ├── Emergencia.cs
│   │   │   ├── Triaje.cs
│   │   │   ├── Seguro.cs
│   │   │   ├── PacienteSeguro.cs
│   │   │   ├── Reclamo.cs
│   │   │   ├── EncuestaSatisfaccion.cs
│   │   │   ├── CampaniaMarketing.cs
│   │   │   ├── PlantillaMensaje.cs
│   │   │   ├── CuponDescuento.cs
│   │   │   ├── PacienteCupon.cs
│   │   │   ├── Referencia.cs
│   │   │   ├── ConsentimientoInformado.cs
│   │   │   ├── CertificadoMedico.cs
│   │   │   ├── IncapacidadTemporal.cs
│   │   │   ├── AuditoriaCita.cs
│   │   │   └── BitacoraAcceso.cs
│   │   │
│   │   ├── Enums/
│   │   │   ├── EstadoCita.cs
│   │   │   ├── EstadoFactura.cs
│   │   │   ├── EstadoPago.cs
│   │   │   ├── EstadoHospitalizacion.cs
│   │   │   ├── PrioridadEmergencia.cs
│   │   │   ├── TipoConsulta.cs
│   │   │   ├── TipoDocumento.cs
│   │   │   ├── TipoNotificacion.cs
│   │   │   ├── MetodoPagoEnum.cs
│   │   │   ├── EstadoComprobante.cs
│   │   │   ├── TipoComprobante.cs
│   │   │   ├── Genero.cs
│   │   │   ├── TipoSangre.cs
│   │   │   ├── EstadoCivil.cs
│   │   │   └── NivelPrioridad.cs
│   │   │
│   │   ├── Interfaces/
│   │   │   ├── Repositories/
│   │   │   │   ├── IRepository.cs
│   │   │   │   ├── IUsuarioRepository.cs
│   │   │   │   ├── IPacienteRepository.cs
│   │   │   │   ├── IMedicoRepository.cs
│   │   │   │   ├── ICitaRepository.cs
│   │   │   │   ├── IFacturaRepository.cs
│   │   │   │   ├── IRecetaRepository.cs
│   │   │   │   ├── IInventarioRepository.cs
│   │   │   │   ├── IHospitalizacionRepository.cs
│   │   │   │   ├── ILaboratorioRepository.cs
│   │   │   │   ├── INotificacionRepository.cs
│   │   │   │   ├── ICampaniaRepository.cs
│   │   │   │   └── IReporteRepository.cs
│   │   │   └── Services/
│   │   │       ├── IAuthService.cs
│   │   │       ├── IEmailService.cs
│   │   │       ├── ISmsService.cs
│   │   │       ├── IWhatsAppService.cs
│   │   │       ├── IPaymentService.cs
│   │   │       ├── ISunatService.cs
│   │   │       ├── ITelemedicinaService.cs
│   │   │       ├── INotificationService.cs
│   │   │       ├── IPdfService.cs
│   │   │       ├── IQrService.cs
│   │   │       ├── IReportService.cs
│   │   │       ├── IDashboardService.cs
│   │   │       ├── IPrioridadService.cs
│   │   │       ├── IDisponibilidadService.cs
│   │   │       ├── IMarketingService.cs
│   │   │       ├── IInventoryService.cs
│   │   │       └── IAuditService.cs
│   │   │
│   │   └── DTOs/
│   │       ├── Auth/
│   │       │   ├── LoginDto.cs
│   │       │   ├── LoginResponseDto.cs
│   │       │   ├── RegistroDto.cs
│   │       │   ├── ChangePasswordDto.cs
│   │       │   ├── ForgotPasswordDto.cs
│   │       │   ├── ResetPasswordDto.cs
│   │       │   └── RefreshTokenDto.cs
│   │       ├── Paciente/
│   │       │   ├── PacienteDto.cs
│   │       │   ├── CreatePacienteDto.cs
│   │       │   ├── UpdatePacienteDto.cs
│   │       │   └── PacienteDetailDto.cs
│   │       ├── Cita/
│   │       │   ├── ReservaCitaDto.cs
│   │       │   ├── CitaDto.cs
│   │       │   ├── CancelarCitaDto.cs
│   │       │   ├── ReprogramarCitaDto.cs
│   │       │   └── CitaDetailDto.cs
│   │       ├── Facturacion/
│   │       │   ├── FacturaDto.cs
│   │       │   ├── CreateFacturaDto.cs
│   │       │   ├── PagoDto.cs
│   │       │   ├── ProcesarPagoDto.cs
│   │       │   ├── PagoResponseDto.cs
│   │       │   └── ComprobanteElectronicoDto.cs
│   │       ├── Receta/
│   │       │   ├── RecetaDto.cs
│   │       │   ├── CreateRecetaDto.cs
│   │       │   ├── DetalleRecetaDto.cs
│   │       │   └── RecetaQrDto.cs
│   │       ├── Telemedicina/
│   │       │   ├── TeleconsultaDto.cs
│   │       │   ├── IniciarTeleconsultaDto.cs
│   │       │   └── VideoCallTokenDto.cs
│   │       ├── Marketing/
│   │       │   ├── CampaniaDto.cs
│   │       │   ├── CreateCampaniaDto.cs
│   │       │   └── CampaniaEstadisticasDto.cs
│   │       ├── Inventario/
│   │       │   ├── ProductoDto.cs
│   │       │   ├── MovimientoDto.cs
│   │       │   ├── StockDto.cs
│   │       │   └── AlertaStockDto.cs
│   │       ├── Laboratorio/
│   │       │   ├── OrdenExamenDto.cs
│   │       │   ├── ResultadoExamenDto.cs
│   │       │   └── ExamenDto.cs
│   │       ├── Hospitalizacion/
│   │       │   ├── CamaDto.cs
│   │       │   ├── HospitalizacionDto.cs
│   │       │   └── AsignarCamaDto.cs
│   │       └── Reportes/
│   │           ├── DashboardDto.cs
│   │           ├── ReporteCitasDto.cs
│   │           ├── ReporteFinancieroDto.cs
│   │           ├── ReporteRecetasDto.cs
│   │           └── PrediccionAusenciasDto.cs
│   │
│   ├── MediTurno.Infrastructure/               # INFRAESTRUCTURA - Datos y Servicios
│   │   ├── Data/
│   │   │   ├── Context/
│   │   │   │   └── ApplicationDbContext.cs
│   │   │   ├── Configurations/
│   │   │   │   ├── UsuarioConfiguration.cs
│   │   │   │   ├── PacienteConfiguration.cs
│   │   │   │   ├── CitaConfiguration.cs
│   │   │   │   └── FacturaConfiguration.cs
│   │   │   ├── Migrations/
│   │   │   └── Seed/
│   │   │       ├── DatabaseSeeder.cs
│   │   │       ├── RoleSeeder.cs
│   │   │       ├── EspecialidadSeeder.cs
│   │   │       └── MedicamentoSeeder.cs
│   │   ├── Repositories/
│   │   │   ├── Repository.cs
│   │   │   ├── UsuarioRepository.cs
│   │   │   ├── PacienteRepository.cs
│   │   │   ├── MedicoRepository.cs
│   │   │   ├── CitaRepository.cs
│   │   │   ├── FacturaRepository.cs
│   │   │   ├── RecetaRepository.cs
│   │   │   ├── InventarioRepository.cs
│   │   │   ├── HospitalizacionRepository.cs
│   │   │   ├── LaboratorioRepository.cs
│   │   │   ├── NotificacionRepository.cs
│   │   │   ├── CampaniaRepository.cs
│   │   │   └── ReporteRepository.cs
│   │   └── Services/
│   │       ├── AuthService.cs
│   │       ├── EmailService.cs
│   │       ├── SmsService.cs
│   │       ├── WhatsAppService.cs                    # WhatsApp Business API
│   │       ├── PaymentService.cs                     # Culqi / Niubiz / Yape
│   │       ├── SunatService.cs                       # Facturación electrónica
│   │       ├── TelemedicinaService.cs                # Videollamadas (Daily/Whereby)
│   │       ├── NotificationService.cs
│   │       ├── PdfService.cs
│   │       ├── QrService.cs
│   │       ├── ReportService.cs
│   │       ├── DashboardService.cs
│   │       ├── PrioridadService.cs
│   │       ├── DisponibilidadService.cs
│   │       ├── MarketingService.cs
│   │       ├── InventoryService.cs
│   │       ├── AuditService.cs
│   │       ├── JwtService.cs
│   │       └── HashHelper.cs
│   │
│   ├── MediTurno.API/                             # API RESTful (para móviles)
│   │   ├── Controllers/
│   │   │   ├── v1/
│   │   │   │   ├── AuthController.cs
│   │   │   │   ├── CitasController.cs
│   │   │   │   ├── PacientesController.cs
│   │   │   │   ├── MedicosController.cs
│   │   │   │   ├── FacturasController.cs
│   │   │   │   ├── PagosController.cs               # Pasarela de pagos pública
│   │   │   │   ├── RecetasController.cs
│   │   │   │   ├── TelemedicinaController.cs
│   │   │   │   ├── InventarioController.cs
│   │   │   │   ├── MarketingController.cs
│   │   │   │   ├── ReportesController.cs
│   │   │   │   └── DashboardController.cs
│   │   │   └── BaseApiController.cs
│   │   ├── Middleware/
│   │   │   ├── ApiKeyMiddleware.cs
│   │   │   ├── RateLimitingMiddleware.cs
│   │   │   └── JwtMiddleware.cs
│   │   ├── Swagger/
│   │   │   └── SwaggerConfig.cs
│   │   └── appsettings.API.json
│   │
│   ├── MediTurno.Web/                              # MVC Web
│   │   ├── Controllers/
│   │   │   ├── AccountController.cs
│   │   │   ├── AdminController.cs
│   │   │   ├── PacienteController.cs
│   │   │   ├── MedicoController.cs
│   │   │   ├── CitaController.cs
│   │   │   ├── FacturaController.cs
│   │   │   ├── PagoController.cs                    # Pasarela de pagos
│   │   │   ├── RecetaController.cs
│   │   │   ├── TelemedicinaController.cs
│   │   │   ├── InventarioController.cs
│   │   │   ├── LaboratorioController.cs
│   │   │   ├── HospitalizacionController.cs
│   │   │   ├── MarketingController.cs
│   │   │   ├── ReporteController.cs
│   │   │   └── HomeController.cs
│   │   │
│   │   ├── Views/
│   │   │   ├── Account/
│   │   │   │   ├── Login.cshtml
│   │   │   │   ├── Registro.cshtml
│   │   │   │   ├── ForgotPassword.cshtml
│   │   │   │   └── ResetPassword.cshtml
│   │   │   ├── Admin/
│   │   │   │   ├── Dashboard.cshtml
│   │   │   │   ├── Usuarios.cshtml
│   │   │   │   ├── Roles.cshtml
│   │   │   │   ├── Configuracion.cshtml
│   │   │   │   ├── Logs.cshtml
│   │   │   │   ├── Especialidades.cshtml
│   │   │   │   ├── Medicos.cshtml
│   │   │   │   ├── Pacientes.cshtml
│   │   │   │   ├── Reportes.cshtml
│   │   │   │   └── Campanias.cshtml
│   │   │   ├── Paciente/
│   │   │   │   ├── Dashboard.cshtml
│   │   │   │   ├── MisCitas.cshtml
│   │   │   │   ├── Perfil.cshtml
│   │   │   │   ├── HistorialClinico.cshtml
│   │   │   │   ├── Recetas.cshtml
│   │   │   │   ├── Facturas.cshtml
│   │   │   │   ├── Telemedicina.cshtml
│   │   │   │   ├── ReservarPaso1.cshtml
│   │   │   │   ├── ReservarPaso2.cshtml
│   │   │   │   ├── ReservarPaso3.cshtml
│   │   │   │   ├── ConfirmarCita.cshtml
│   │   │   │   └── Pago.cshtml
│   │   │   ├── Medico/
│   │   │   │   ├── Dashboard.cshtml
│   │   │   │   ├── MisCitas.cshtml
│   │   │   │   ├── Agenda.cshtml
│   │   │   │   ├── AtencionCita.cshtml
│   │   │   │   ├── HistorialPaciente.cshtml
│   │   │   │   ├── Recetario.cshtml
│   │   │   │   ├── RecetaElectronica.cshtml
│   │   │   │   ├── Teleconsulta.cshtml
│   │   │   │   ├── Examenes.cshtml
│   │   │   │   └── Horarios.cshtml
│   │   │   ├── Shared/
│   │   │   │   ├── _Layout.cshtml
│   │   │   │   ├── _LayoutAdmin.cshtml
│   │   │   │   ├── _LayoutPaciente.cshtml
│   │   │   │   ├── _LayoutMedico.cshtml
│   │   │   │   ├── _Alertas.cshtml
│   │   │   │   ├── _Sidebar.cshtml
│   │   │   │   ├── _Navbar.cshtml
│   │   │   │   ├── _Footer.cshtml
│   │   │   │   └── Error.cshtml
│   │   │   └── Home/
│   │   │       └── Index.cshtml
│   │   │
│   │   ├── ViewModels/
│   │   │   ├── Auth/
│   │   │   │   ├── LoginViewModel.cs
│   │   │   │   └── RegistroViewModel.cs
│   │   │   ├── Admin/
│   │   │   │   ├── DashboardViewModel.cs
│   │   │   │   └── UsuarioViewModel.cs
│   │   │   ├── Paciente/
│   │   │   │   ├── PerfilViewModel.cs
│   │   │   │   ├── CarritoCitaViewModel.cs
│   │   │   │   └── PagoViewModel.cs
│   │   │   └── Medico/
│   │   │       ├── AtencionViewModel.cs
│   │   │       └── RecetaViewModel.cs
│   │   │
│   │   ├── Middleware/
│   │   │   ├── ErrorHandlingMiddleware.cs
│   │   │   ├── SessionValidationMiddleware.cs
│   │   │   └── AuditLogMiddleware.cs
│   │   │
│   │   ├── Filters/
│   │   │   ├── AuthorizeUserFilter.cs
│   │   │   ├── ValidateModelFilter.cs
│   │   │   └── PerformanceFilter.cs
│   │   │
│   │   ├── wwwroot/
│   │   │   ├── css/
│   │   │   │   ├── site.css
│   │   │   │   ├── admin.css
│   │   │   │   └── dark-mode.css
│   │   │   ├── js/
│   │   │   │   ├── site.js
│   │   │   │   ├── dashboard.js
│   │   │   │   ├── calendar.js
│   │   │   │   ├── chart.js
│   │   │   │   ├── payment.js
│   │   │   │   └── webrtc.js
│   │   │   ├── lib/
│   │   │   │   ├── bootstrap/
│   │   │   │   ├── font-awesome/
│   │   │   │   ├── fullcalendar/
│   │   │   │   ├── chart.js/
│   │   │   │   └── datatables/
│   │   │   └── uploads/
│   │   │       ├── recetas/
│   │   │       ├── examenes/
│   │   │       ├── perfiles/
│   │   │       └── comprobantes/
│   │   │
│   │   ├── Program.cs
│   │   └── appsettings.json
│   │
│   └── MediTurno.Tests/                           # Pruebas
│       ├── UnitTests/
│       │   ├── Services/
│       │   │   ├── PrioridadServiceTests.cs
│       │   │   ├── PaymentServiceTests.cs
│       │   │   └── MarketingServiceTests.cs
│       │   └── Controllers/
│       │       ├── AccountControllerTests.cs
│       │       └── CitaControllerTests.cs
│       ├── IntegrationTests/
│       │   └── CitaIntegrationTests.cs
│       └── xunit.runner.json
│
├── Scripts/                                       # Scripts SQL
│   ├── 01_CreateDatabase.sql
│   ├── 02_StoredProcedures.sql
│   ├── 03_SeedData.sql
│   ├── 04_Indexes.sql
│   └── 05_Triggers.sql
│
├── docker-compose.yml
├── .env
└── README.md


✅ RESUMEN DE NUEVAS FUNCIONALIDADES IMPLEMENTADAS
Módulo	Funcionalidades	Tecnología
Pasarela de Pagos	Culqi, Yape, PLIN	API Culqi, QR
Facturación Electrónica	Boletas/Facturas SUNAT	API SUNAT, PDF, XML
WhatsApp Business	Recordatorios, promociones, confirmaciones	Meta WhatsApp API
Telemedicina	Videoconsultas, salas virtuales	Daily/Whereby API
Marketing Automation	Campañas, cumpleaños, fidelización	Email, WhatsApp, SMS
Recetas Electrónicas	QR, envío a farmacia, firma digital	PDF, QRCoder
Inventario/Farmacia	Stock, caducidades, compras	ADO.NET
Laboratorio	Órdenes de exámenes, resultados	Sistema integrado
Hospitalización	Camas, quirófanos, cirugías	Gestión completa
Dashboard IA	Predicción de ausencias	ML.NET
Reportes Avanzados	Financieros, productividad, tendencias	Chart.js, Excel

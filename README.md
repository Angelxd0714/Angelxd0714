# 👨‍💻 **Angel Santibañez** | Desarrollador Backend | Colombia 🇨🇴  

`System.out.println("Transformando café en código eficiente ☕→💻");`  

## 🚀 **Sobre Mí**  
Desarrollador backend especializado en arquitecturas escalables con **Spring Boot** y **Django**. Apasionado por crear soluciones robustas con altos estándares de calidad y performance.  

## 🛠 **Tecnologías Principales**  

### 🔷 **Lenguajes**  
<p align="left">
  <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java"/>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript"/>
</p>

### 🏗 **Frameworks**  
<p align="left">
  <img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white" alt="Spring Boot"/>
  <img src="https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white" alt="Django"/>
</p>

### ☁ **Cloud & DevOps**  
<p align="left">
  <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white" alt="AWS"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker"/>
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" alt="Kubernetes"/>
</p>

## 📊 **Mis Estadísticas**  

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Angelxd0714&show_icons=true&theme=radical&include_all_commits=true" alt="Estadísticas" width="48%"/>
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=Angelxd0714&theme=radical" alt="Racha" width="48%"/>
</div>

## 🔥 **Proyectos Destacados**  

### 🏥 **Sistema Hospitalario SUAP (Django)**  
![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)  
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)  

**Características:**  
- ✅ Gestión multiusuario (Médicos, Enfermeros, Pacientes)  
- ✅ Sistema de citas médicas con notificaciones  
- ✅ Generación de reportes en PDF  
- ✅ Integración con pasarelas de pago  

### 💳 **Microservicio de Pagos (Spring Boot)**  
![Spring](https://img.shields.io/badge/Spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white)  
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white)  

**Logros:**  
- 🚀 Implementación de JWT para seguridad  
- 🔁 Arquitectura reactiva con WebFlux  
- 📈 Escalabilidad en AWS EKS  

## 📫 **Conéctate Conmigo**  

<p align="center">
  <a href="mailto:tu-email@example.com">
    <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" height="30"/>
  </a>
  <a href="https://linkedin.com/in/tu-perfil">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" height="30"/>
  </a>
  <a href="https://discord.com/users/tu-id">
    <img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" height="30"/>
  </a>
</p>

## 💻 **Código de Ejemplo**  

```java
@RestController
@RequestMapping("/api/v1/payments")
public class PaymentController {
    
    private final PaymentService paymentService;

    @PostMapping
    public Mono<PaymentResponse> processPayment(@Valid @RequestBody PaymentRequest request) {
        return paymentService.processPayment(request);
    }

    @GetMapping("/{id}")
    public Mono<PaymentDetails> getPaymentDetails(@PathVariable String id) {
        return paymentService.getPaymentDetails(id);
    }
}

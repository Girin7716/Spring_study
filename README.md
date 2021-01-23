# Spring

https://www.inflearn.com/ ���� '������ �Թ� - �ڵ�� ���� ������ ��Ʈ, �� MVC, DB ���� ���_�迵��' ���Ǹ� ���� �����ߴ�.

---
---
## ���� 0. ���ǼҰ�

---
---

### ������ �� ���ø����̼� ����

- ������ ������Ʈ ����
- ������ ��Ʈ�� �� ���� ����
- ȸ�� ������ ����
- �� MVC ����
- DB ���� - JDBC, JPA, ������ ������ JPA
- �׽�Ʈ ���̽� �ۼ�

---

### ������Ʈ �����

- Spring Boot
- Gradle
- Thymeleaf
- HIBERNATE
- JPA

---

### ���� ��ǥ

- ������ �н��� ����� �� ù ������ ����
- ������ ��� �� ��ü�� �Ÿ� X
- ��� ����ؾ� �ϴ����� ����
- ������ ������ ��� X
- ���̳��� ������ ��� X

---

### ������ ���� ���� �ε��

- ������ �Թ�
- ������ �ٽ� ����
- ������ �� MVC
- ������ DB ������ ���� ���
- ����! ������ ��Ʈ


---
---

## ���� 1. ������Ʈ ȯ�漳��

---
---

### ������ ��Ʈ ��Ÿ�� ����Ʈ�� �̵��ؼ� ������ ������Ʈ ����

- �������� ������ ������Ʈ�� �عٴں��� ���������, ������ ������ ��Ʈ�� ������� ������ ������Ʈ�� ����.
- https://start.spring.io
  ![start.spring.io](./readme_img/start_spring.JPG)

- Project
  - �ʿ��� ���̺귯���� ���ܼ� ����, �갡 �����ϴ� ����������Ŭ���� �������ִ� ��
  - �������� Maven, ������ Gradle�� �Ѿ�� �߼�
  - ![gradle](./readme_img/gradle.JPG)

- Language
  - Java
- Spring Boot
  - ������ ������ �ؾ���
  - SNAPSHOT
    - ����� �ִ� ����
  - M1 ...
    - ���� ������ ������ �ƴ�
  - ���� ������ ���� �� ���� ���ƺ��̴� 2.4.2�� ����
    ![2_4_2](./readme_img/2_4_2.JPG)
- Project Metadat
  - Group
    - ���� ������� ����
  - Artifact
    - ����Ǿ� ���ö� ������ �����(������Ʈ ��� ���)
  - �׿ܴ� �׳� ����
  ![project_metadata](./readme_img/project_metadata.JPG)
- Dependencies
  - �̰� �߿���.
  - Spring boot ������� ������Ʈ�� �����Ұǵ� � ���̺귯���� ���ܼ� ����� ���ΰ��� ���� ����
  - ���⼭�� web project�� ����Ŵϱ� 'spring web'�� 'thymeleaf'�� �߰�
    ![spring_web](./readme_img/spring_web.JPG)<br/>
    ![thymeleaf](./readme_img/thymeleaf.JPG)
    - thymeleaf
      - html�� ������ִ� ���ø� ����.

![dependencies](./readme_img/dependencies.JPG)

- �� ��, Generate�� ������ �ٿ�ε带 �ް� �ȴ�.<br/>
    ![hello-spring](./readme_img/hello-spring.JPG)
    - ���� ���ϴ� ������ �ű� �� ������ Ǯ�� '���ڸ�����'���� ����
    - ���� Ǭ ��η� ���� build.gradle�� ������ Open
    - 

---

### ��ġ �� ���ڸ����̿��� ���� ���캸��

- gradle ����
  - gradle ���� ������
- src ����
  - main
    - java
      - ���� package�� �ҽ� ������ ����.
    - resources
      - ���� �ڹ� �ڵ� ������ ������ xml �̳� properties�� ��������, html ���� ������.
  - test
    - test code��� ���õ� �ҽ����� ��.
    - ���� ���� Ʈ���忡�� test code�� �߿���
  - build.gradle
    - �̰� �߿���.
    - ���߿� ��� �����ϰ� ������ gradle�� ���� ������ �ϰ� ���̺귯���� ���ܿ´� ������ ����.
    - ![gradle_version](./readme_img/gradle_version.JPG)
      - sourceCompatibility = '11' �� Java 11 ������ �ǹ�.
    - dependencies
      - ![d_j](./readme_img/dependencies_J.JPG)
      - implementation
        - �Ʊ� �߰��� �͵�
      - testImplementation
        - �⺻������ test ���̺귯���� �ڵ����� ��.
      - ![d_junit](./readme_img/d_junit.JPG)
        - ������ �𸣰����� testImplementation �ؿ� exclude�� �ڵ����� �������־ �׳� ���� ����.
    - repositories
      - �� dependencies�� ���̺귯���� �ٿ�޾ƾ��ϴµ� mavenCentral()�̶�� ������ ����Ʈ���� �ٿ�ε� �޾ƶ��� ������ ��.
  - .gitignore
    - �ҽ��ڵ� �������ִ� ��
    - git���� �ʿ��� �ҽ��ڵ� ���ϸ� �ö󰡰� build�� ������� �ö󰡸� �ȵǴϱ� �����ϴ� ������ start.io���� �� ������ ������
  - settings.gradle
    - ���߿� gradle ��ﶧ �����ϱ�
  
---

### �ѹ� ��������

- ![main_hello_spring](./readme_img/main_hellospring.JPG)
  - �� ��η� �� ��
- ![hellospring_code](./readme_img/hellospring_code.JPG)
  - �̷��� �ڵ���� ���´�.
- ![run_hello](./readme_img/run_hello.JPG)
- ���� �� �̷��� ȭ���� �۵��� ���´�.(�߿�)
  - ![console_After_run](./readme_img/console_after_run.JPG)
    - �ؿ��� �ι�° �� tomcat���� http�� port 8080���� ��.
- �� ��, localhost:8080 �����ϸ� �Ʒ��� ���� ��.
  - ![local8080](./readme_img/local8080.JPG)

- ������� ���������� ������Ʈ ȯ�� ������ ����.
---

### ���̺귯�� ���캸��

����ϰ� ���캽

- ![ex_lib](./readme_img/external_lib.JPG)
  - ������ ������ ����.
  - gradle�̳� maven ���� build ������ �������踦 �� ������ ����
    - ex>�츮�� start.sprnig.io���� �߰��� spring-booter-starter-web�� ����� �̰��� �ʿ��� ���̺귯���� ��Ĺ, spring web, spring MVC �̷��͵��� ���ܿ�(== �������踦 ����)
      - �츮�� spring-booter-starter-web�� �ʿ������� �� spring-booter-starter-web�� �ʿ��� �͵鿡�� ������ �ϰ� �ִ�.
      - �׷��� gradle�� ������ ���� �� ģ������ ���� ���ܿ´�.

- '���ڸ�����' �����ʿ� ���� gradle�� �ִµ� �̰� Ŭ���ϸ� �Ʒ��� ���� ���´�.
  - ![right_gradle](./readme_img/right_gradle.JPG)
  - Dependencies
    - ���̺귯������� ��������
    - ![look_gradle](./readme_img/look_gradle.JPG)
      - ���� thymeleaf �� web �� 2���� ���ܿԾ���.
    - ![recur_gradle](./readme_img/recur_gradle.JPG)
      - ������ �� ���� ó�� �������� �ʿ��� ���̺귯���� ������ ������ ���� ��� ���ܿ�
    - tomcat
      - web server�� ����� ��
      - �������� WAS(or Web Server)�� ���� ������ ��ġ(tomcat ������), �׸��� �ű⿡ �ڹ� �ڵ带 ����ִ´�.
        - �������� ���� ���̺귯���� �и��� �Ǿ� �־���.
        - �ǰ� ���� �۾������� ���򿡴� �ҽ� ���̺귯������ �������� ����ִ�(==�Ӻ����(Ȥ�� �����ϰ� �ִ�.)) �� ���ุ �ϴµ��� �������� ��.
        - ![tomcat_imb](./readme_img/tomcat_imb.JPG)
- log ����
  - ���������� System.out.println���� ����ϸ� �ȵ� �� log��� �ɷ� ����ؾ���.
    - �׷��� log�� ���ܾ� �ɰ��� �͵��� ���� ���� �� log ������ ���� �����ؼ� �� �� ����.
  - ![gradle_log](./readme_img/gradle_log.JPG)
    - slf4j == �������̽�
    - ���� log�� � ����ü�� ����� ���ΰ��� ���� logback�� ���� ������.
    - log �����ؼ� �ñ��Ѱ� ������ �� 2���� �˻��ؼ� �˾ƺ���

- test ���� ���̺귯��
  - junit
    - java���� test�Ҷ� junit ���̺귯���� ���� ����Ѵ�.

- ���(�ٽ� ���̺귯�� �� �����ڷῡ ����)
  - ������ ��Ʈ ���̺귯��
    - spring-boot-starter-web
      - spring-boot-starter-tomcat: ��Ĺ (������)
      - spring-webmvc: ������ �� MVC
    - spring-boot-starter-thymeleaf: Ÿ�Ӹ��� ���ø� ����(View)
    - spring-boot-starter(����): ������ ��Ʈ + ������ �ھ� + �α�
      - spring-boot
        - spring-core
      - spring-boot-starter-logging
        - logback, slf4j
  - �׽�Ʈ ���̺귯��
    - spring-boot-starter-test
        - junit: �׽�Ʈ �����ӿ�ũ
        - mockito: �� ���̺귯��
        - assertj: �׽�Ʈ �ڵ带 �� �� ���ϰ� �ۼ��ϰ� �����ִ� ���̺귯��
        - spring-test: ������ ���� �׽�Ʈ ����
---

### View ȯ�漳��

- Welcome Page �����
  - ![index.html](./readme_img/index_html.JPG)
  - localhost:8080�� �����ϸ� �Ʒ��� ���� ��.
    ![hello_hello](/.readme_img/hello_hello.JPG)
  - hello �� ������ �ƹ��͵� �����Ƿ� ������ ��.
    ![hello_error](./readme_img/hello_error.JPG)
- Spring ����� ��û ���� spring.io ���� �ʿ��� �� ã�� �ɷ��� �߿���.
  - ex> Welcome Page ����
    - spring.io �� Project �� Spring Boot �� LEARN �� 2.4.2 ���� Reference Document Ŭ�� �� Spring Boot Features �� ctrl+F �� welcome page �˻�
      ![search_welcome](./readme_img/search_welcome.JPG)
    - �ٵ� �̰Ŵ� ����(static)��.
- ���ø� ����
  - ���ø� ������ ����ϸ� �����̾ƴ� �������� �������� �ٲ� �� ����.
  - ���⼭�� thymeleaf ���ø� ���� ���.
  - thymeleaf ���� ����Ʈ: https://www.thymeleaf.org/
  - ������ ���� Ʃ�丮��: https://spring.io/guides/gs/serving-web-content/
  - ��������Ʈ �޴���: https://docs.spring.io/spring-boot/docs/2.3.1.RELEASE/reference/html/spring-boot-features.html#boot-features-spring-mvc-template-engines


---

### Controler

- ![controller](./readme_img/controller.JPG)
  - hello.hellospring �ȿ� 'controller' ��� Package ����
    - 'controller' Package�ȿ� 'HelloController' ��� Java Class ����
- Controller Class�� @Controller�� ���� ���������.(�Ʒ� �������� ���� �� 'Controller'��� ������)
  - @�� Annotatino�̶�� ��.
  - ![append_controller](./readme_img/append_controller.JPG)

- ![getmapping](./readme_img/getmapping.JPG)
  - @GetMapping(~~)
  - �� ���ø����̼ǿ��� /hello ��� ������ �Ʒ��� method�� ȣ�����ش�.
- �Ʒ��� ���� �ڵ� �ۼ�
    ```java
    package hello.hellospring.controller;

    import org.springframework.stereotype.Controller;
    import org.springframework.ui.Model;
    import org.springframework.web.bind.annotation.GetMapping;

    @Controller
    public class HelloController {
        @GetMapping("hello")
        public String hello(Model model){
            model.addAttribute("data", "hello!!");
            return "hello";
        }
    }

    ```
- �� ��, src/resources/templetes/ �� hello.html ����
  - ![templete_hello](./readme_img/templete_hello.JPG)
  - ���� �ڷῡ �ִ� �ڵ� ����
    - ![hello_html](./readme_img/hello_html.JPG)
  
- ![html_th](./readme_img/html_th.JPG)
  - xml ��Ű���� ���ø� ������ ������ �Ǿ��ִ� ���.
  - �̷��� ���ø� ������ thymeleaf ������ ����� �� �ִ�.
- ![p](./readme_img/p.JPG)
  - "${data}" �� �Ʊ� Controller�� �ۼ��� model.addAttribute���� key�־��� "data"�� value�� "hello!!"�̴�.
    - ��, "${data}" �� "hello!!"�� ġȯ.
  - ![local_hello](./readme_img/local_hello.JPG)
- ![environment](./readme_img/environment.JPG)
  - @GetMapping������ Get�� Get / Post �Ҷ� �� Get��
    - http url �� ���Ƿ� ġ�� ����ġ�� �װ� Get ����̶�� ��.
    - �׷��� controller�� �ִ� �ش� method�� ������ ��.
    - Spring�� Model�̶�� ���� ���� �Ű������� �־���.
    - model���ٰ� addAttribute�ؼ� key�� "data", value�� "hello!"�� �־��ش�.
    - �׸��� "hello"�� �������ش�.
      - ![return_hello](./readme_img/return_hello.JPG)
        - return "hello"�� �ǹ̴� resources/templetes/hello�� ���� model�̶�� ���� �Ѱܶ�.
    - mapping ��δ� resources:templates/'+{ViewName}+'.html'�̴�.
- ����: spring-boot-devtools ���̺귯���� �߰��ϸ�, html ������ �����ϸ� ���ָ� ���� ����� ���� View ���� ������ �����ϴ�.
- ���ڸ�J ������ ���: �޴� build Recompile

---

### �����ϰ� �����ϱ�

- ���ǿ����� �� �͹̳η� �����ؼ� ���� wsl2�� ������. �� windown�� wsl2���� java ȯ�溯�� ������ �ȵǾ �׳� cmdâ���� ������(<strong>git bash</strong>�� �ϴ°� �� ���ѵ�)
  - gradlew + enter �� gradlew build + enter
  - �� �� build/libs �� ����
    - ![build/libs](./readme_img/build_libs.JPG)
  - �� ��, java -jar hello-spring-0.0.1-SNAPSHOT.jar �� �Է��ϸ� console���� �� jar ������ ������ ��.
- ��, ������ �����Ҷ��� �� jar ���ϸ� �����ؼ� ������ �ְ� �ű⿡�� java -jar�� �����Ű�� �������� spring�� ������ ��.

- ./gradlew clean build
  - build ������ ������
- 

---
---
## ���� 2. ������ �� ���� ����
---
---

### ���� �����Ѵٴ� ��
  1. ���� ������
     - �������� �� �ϴ°� ���� �׳� ������ �״�� ���������� ������  
  2. MVC�� ���ø� ����
     - ���� ���� �ϴ� ���
     - jsp, php �� �̰͵��� ���ø� ����
     - Model-View-Controller �������� ������ 
     - server���� �����ؼ� <strong>html</strong>�� �ٲ㼭 �����ִ� ���
  3. API ���
     - �ȵ���̵峪 ������ client�� �����ϸ� ���������� <strong>json</strong>�̶�� data format���� ������ 
     - api�� data�� �����ָ� ȭ���� client�� �˾Ƽ� �׸��� �����ϴµ� �̶� api����� ���� ���
     - �������� ����Ҷ� html�� �ְ���� �ʿ� ���� data�� �ְ� �ޱ� ���� �����

---

### ���� ������
  - spring boot�� ���� ������ ����� �⺻������ ����
  - resources/static/ ���� hello-static.html �����ؼ� �����ڷῡ �ִ� �ڵ� ����
  - ![static_contents](./readme_img/static_contents.JPG)
  - ![static_contents_img](./readme_img/static_contents_img.JPG)
    - �� ���������� localhost:8080/hello-static.html ġ��<br/> 
      1) ���� ���� ������ ��û�� �ް�
      2) hello-static.html�� �Դٴ� ���� spring���� �ѱ� 
      3) spring�� controller�ʿ��� hello-static�̶�� ���� �ִ��� ã�ƺ���(controller�� �켱������ �����ٴ� ��) 
      4) hello��� controller�� �־����� hello-static�̶�� controller�� ���� 
      5) ������ �� ���� resources:static/hello-static.html �̶�� ���� ã�´�. 
      6) �׷��� �ؼ� ������ �װ��� ��ȯ����

---

### MVC�� ���ø� ����

  - MVC == Model-View-Controller
  - ���ſ��� controller�� view�� ���� �и��Ǿ� ���� �ʰ� view���� ������ ����
    - jsp�� asp �׷��� ���� ��
    - �̸�, Model one ����̶�� ��
    - �̷����ϸ� �������� �ʹ� �����. view ���Ͽ��� ��õ ���� �ڵ尡 �ȴ�.
  - ���򿡴� MVC ������� ���� ��.
    - ���ɻ縦 �и��ؾ��ϱ� ������(���Ұ� å��)
    - View�� ȭ���� �׸��µ��� ����
    - Model �̳� Controller�� ���� business logic�̳� �������� ��(�鿣��)�� ó���ϴµ� ����.
    - �׷��� �鿣�忡�� ó���� �Ͽ��� ȭ��(View)���� �ʿ��� �������� model�̶�� �Ϳ� ��Ƽ� �Ѱ��ִ� ������ ���� ���.
- ![hello-empty](./readme_img/hello-empty.JPG)
  - ���⼭ hello! empty�� ���ø� �������μ� ������ �ϸ� ������ ������ ������ ġȯ, ���ø� �������μ� ������ ���ϸ�(�������� ������ ��η� ���� �� ���) hello! empty ���

- controller���ٰ� �߰���
    ```java
    @GetMapping("hello-mvc")
        public String helloMvc(@RequestParam("name") String name, Model model){
            model.addAttribute("name",name);
            return "hello-template";
        }
    ```
    �� �Է��ϰ�, localhost:8080/hello-mvc�� ġ�� ������ ��.
    - ������ ���� �ϴ� log�� ������.
      - ![warning](./readme_img/warning.JPG)
      - ![warning_name](./readme_img/warning_name.JPG)
    - @RequestParam("name")���� Ŀ�� �̵� �� Ctrl+P ������ �Ķ���� ������ �� �� ����
  - localhost:8080/hello-mvc?name=spring�� �Է��ϸ� http GET ��Ŀ��� ? ~~~ �� parameter�� �Ѱ��� �� ����.
    - �׷��� name�� spring�� �Ѱ��־ ������ ���� ����� ���´�.
    - ![get](./readme_img/get.JPG)
  - ![mvc_img](./readme_img/mvc_img.JPG)
    - ������������ localhost:8080/hello-mvc�� �ѱ��
      1) ���� ���� ������ ���ļ� spring���� hello-mvc��� ���� �Դٰ� ������
      2) spring�� helloController�� �� method�� mapping�� �Ǿ� �־ �� method�� ȣ�����ش�
      3) return�� "hello-template" model(name:spring) �̷��� spring���� �Ѱ��ش�
      4) viewResolver(ȭ��� ���õ� �ذ���, view�� ã���ְ� ���ø� ������ ���� ������)�� templates/hello-template.html�� ã�Ƽ� thymeleaf ���ø� ������ ó���ش޶�� �ѱ�.
      5) ���ø� ������ �������� �ؼ� ��ȯ�� �� html�� �� �������� ��ȯ�� �Ѵ�.(�����϶��� �̶�, ��ȯ�� ���� �ʰ� ��ȯ)
  - ![look_source_mvc](./readme_img/look_source_mvc.JPG)

---

## API ���

- �ϴ� �ڵ�
  - ���������� controller�� �Ʒ� �ڵ� �߰�
    ```java
    @GetMapping("hello-string")
    @ResponseBody
    public String helloString(@RequestParam("name") String name){
        return "hello " + name;
    }
    ``` 
    - @ResponseBody�� http ��� �������ݿ��� header�� body�� �ִµ� body�� �� data�� ���� ���� �־��ְڴٶ�� ��.(html������ body �±װ� �ƴ�)
    - ���ø� �������� ���̴� View �̷��� ���� ���ڰ� �״�� ������.
    - �����ϸ� �Ʒ��� ���� ����.
        ![api](./readme_img/api.JPG)
    - �ڵ带 ���� �̷��� ����
        ![api_string](./readme_img/api_string.JPG)
        - �׳� ���ڰ� �״�� ������.(��, view ���� �״�� ������)
        - �ٵ� �̷��Դ� ���� �� �� ����
- ���� data�� ����� ��(�̰� ������ api ����� ���� ���)
  - �ϴ� �ڵ�
    ```java
    @GetMapping("hello-api")
    @ResponseBody
    public Hello helloApi(@RequestParam("name") String name){
        Hello hello = new Hello();
        hello.setName(name);
        return hello;
    }

    static class Hello{
        private String name;

        public String getName() {
            return name;
        }

        public void setName(String name) {
            this.name = name;
        }
    }
    ``` 
    - return�� class�� �Ѱ��ش�.
    - class���� getter�� setter�� �־�� �ϴµ� �̴� ctrl+insert(������ ��� ctrl+function+delete)�� �����༭ getter and setter Ŭ��
    - �����, ���ڸ����̿��� �ڵ��ϼ� ����Ű�� ctrl+shift+enter �̴�.
    - getter, setter �� java bin �Ծ��̶�� ��
      - private String name ���� ��� private�̴ϱ� �ܺο��� �� �����ϱ� �ܺο��� ����ҷ��� �̷��� getter�� setter�� ���ؼ� ������ �ϰ� ��.
      - property ���� ����̶�� ��.
  - �� �� �����ϸ�, �Ʒ��� ���� ����
    - ![api_json](./readme_img/api_json.JPG)
      - json�̶� ������ �����ϸ� key:value�� �̷���� ����.
  - spring ���� ��� ��ü�� ��ȯ�ϰ� @ResponseBody�� ����θ� �׷��� json���� ��ȯ�ϴ°� default��.(xml���ε� �� ���� ����. �ٵ� ������ �� �Ȼ���Ѵ�.)

- @ResponseBody ��� ����
  - ![api_img](./readme_img/api_img.JPG)
    - �� ���������� ���� localhost:8080/hello-api�� �Է��ϸ�
      1) ���� ���� �������� hello-api�� �Դٰ� spring���� ����.
      2) spring�� controller�� hello-api�� ã�� ã�Ҵµ� @ResponseBody��� annotation�� �پ�������(�� �پ� ������(��, ���ø� �������) viewResolver���� ������) �̶� ��ȯ�ϴ� ���� ��ü�� ���� json ������� �����͸� ���� http ���信 ��ȯ�ϰڴ�(�̰� �⺻ ��å)<br/>
      return: hello(name:spring)
      3) HttpMessageConverter��� ���̰� ������ ��.
         1) �ܼ� �����̴� �� StringConverter�� ����(���� �̸��� StringHttpMessageConverter)
         2) ��ü�̴� �� JsonConverter�� ����(���� �̸��� MappingJackson2HttpMessageConverter)
            - ��ü�� json ��Ÿ�Ϸ� �ٲ۴�.
            - Jackson�̶� ��ü�� json���� �ٲ��ִ� ���̺귯��
              - ��ü�� json���� �ٲ��ִ� ������ ���̺귯���� jackson�� gson�� �̷��� �ִ�.
      4) �ٲ� json�� ��û�� ���� Ȥ�� ������������ �ش�.

- ����
  - ���� ������
    - �׳� ������ �״�� �����ش�.
  - MVC �� ���ø� ����
    - ���ø� ������ Model-View-Control ������� �ɰ��� ���� View�� ���ø� �������� html�� �������ؼ� �������� �� html�� client���� �������ش�.
  - API
    - ��ü�� ��ȯ�ؼ� httpmessageconverter�� ���ؼ� json ���Ϸ� ��ȯ �� ��ȯ�� ����
    - view �̷��� ���� �ٷ� http response�� �ٰ� �ٷ� ��.

---
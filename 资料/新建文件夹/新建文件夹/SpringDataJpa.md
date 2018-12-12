# Ŀ¼���
[TOC]
# ǰ��
&emsp;&emsp;JPA ������Ե����Ϊ�����ϵ����� ORM ��ܣ�����һ�ֱ�׼��[�ٶȰٿ�](https://baike.baidu.com/item/JPA)˵ JDK Ϊ��ʵ�� ORM �����¹�һ���ƶ��� JPA ��һ�ױ�׼��ĿǰҲ���ڰ����������չ�����ǻ�û����ȫʵ�֡��� ORM ����У�Hibernate ��һ֧�ܴ�Ĳ��ӣ��ܷ��㣬����Ҳ��ǿ��ͬʱ��Hibernate Ҳ�� JPA ���ϵıȽ����ã����ǿ�����Ϊ JPA �Ǳ�׼����ʵ��Ҳ�ǣ�JPA ����ȫ�ǽӿڣ�ʵ�ֶ��� Hibernate ����������Ͽ����� JPA ��ͳһ֮�£�Hibernate Ŀǰ�����õ������š�
<br>
&emsp;&emsp;ǰ������� JPA �� Hibernate �Ĺ�ϵ����ô Spring Data JPA ����ʲô�����أ���ط���Ҫ��΢����һ�£������� Java �����Ķ�֪�� Spring ��ǿ�󣬵�ĿǰΪֹ����ҵ��Ӧ�� Spring �������������ܣ��������ڣ��Ѿ�����ʵ�ϵı�׼�ˣ���ҵ��Ӧ�ò����� Spring �ļ���û�У�����˵û��ɣ��� Spring ���ϵ�������ܵ������ֺ�ǿ����Ҫ���Ĳ������Ǹ������ IOC ������ô�򵥵�һ���£����� Spring �漰����ܹ㣬��Ҫ�����ں͵��������ߵ������ϡ�����������������ⷽ�棬Spring ���˳־û���һ��Ĺ��������˸о� Spring ϣ���ѳ־û���һ������Ҳ���£����Ǿ����� Spring Data ϵ�У����� spring-data-jpa��spring-data-template��spring-data-mongodb��spring-data-redis�����и�����Ʒ mybatis-spring����ǰ�����ƣ����Ǻ� MyBatis ���ϵĵ�����������Щ���ǳ־û����߸ɵ��¶���
<br>
&emsp;&emsp;��ѧϰ Spring Data JPA ֮ǰ���ȶ� ORM ˼�� �� JPA ��׼����һ���򵥵��˽⣬��Ϊ Spring Data JPA �ǽ����� ORM ˼��� JPA ��׼֮�ϵ�һ���־ò��ܡ�

# 1. ORM ����
&emsp;&emsp;�����ϵӳ�䣨Object Relational Mapping����� ORM��ORM ��һ��Ϊ�˽������������ϵ���ݿ���ڻ���ƥ�������ļ������򵥵�˵��ORM ��ͨ���������������֮��ӳ���Ԫ���ݣ��������еĶ����Զ��־û�����ϵ���ݿ��С�

# 2. JPA ����
&emsp;&emsp;JPA �� **J**ava **P**ersistence **A**PI �ļ�ƣ����ķ��룺Java �־ò� API������ JDK5.0 ע��� XML ��������������ݿ���ӳ���ϵ�����������ڵ�ʵ�����־û������ݿ��С�
<br>
Sun �����µ� JPA ORM �淶��������ԭ��
- ������ JavaEE �� JavaSE Ӧ�ÿ�������
- Sun ϣ������ ORM ������ʵ�����¹�һ
<br>
��ͼչʾ�� JPA �淶�� ORM ���֮��Ĺ�ϵ


JPA ��������3������ļ�����
- ORM ӳ��Ԫ����
JPA ֧�� JDK5.0 ע��� XML ����Ԫ���ݵ���ʽ��Ԫ������������ͱ�֮���ӳ���ϵ����ܾݴ˽�ʵ�����־û������ݿ���С�
<br>
- API
��������ʵ�����ִ����ɾ�Ĳ����������ں�̨�������������е����飬ʹ�����ߵ��Դӷ����� JDBC �� SQL �����н��ѳ�����
<br>
- ��ѯ����
���ǳ־û������к���Ҫ��һ���֣�ͨ�������������������ݿ�SQL��ѯ���ݣ����������SQL������ϡ�

## 2-1. JPA ������
- ��׼��
JPA �� JCP ��֯������ JavaEE ��׼֮һ������κ����Ʒ��� JPA ��׼�Ŀ�ܶ���ѭͬ���ļܹ����ṩ��ͬ�ķ��� API���Ᵽ֤�˻��� JPA ��������ҵӦ���ܹ������������޸ľ��ܹ��ڲ�ͬ�� JPA ��������С�
<br>
- �򵥷���
JPA ����ҪĿ��֮һ�����ṩ�򵥵ı��ģ�ͣ��� JPA ����´���ʵ��ʹ��� Java ��һ���򵥣�û���κε�Լ�������ƣ�ֻ��Ҫʹ�� javax.persistence.Entity ����������JPA �Ŀ�ܺͽӿ�Ҳ�ǳ��򵥣�û��̫���ر�Ĺ�������ģʽ��Ҫ�󣬿����߿��Ժ����׵����ա�JPA ���ڷ�����ʽ���ԭ����˿��Ժ����׵ĺ�������ܻ����������ɡ�
<br>
- ��ѯ����
JPA �Ĳ�ѯ�����������������������ݿ�ģ���������������Ȼ�﷨�����ѯ��䣬���Կ����� Hibernate HQL �ĵȼ��JPA �����˶��ص� JPQL��Java Persistence Query Language����JPQL �� EJBQL ��һ����չ���������ʵ���һ�ֲ�ѯ���ԣ���������ʵ�壬�����ǹ�ϵ���ݿ�ı������ܹ�֧���������º��޸ġ�join��group by��having ��ͨ��ֻ���� SQL ���ܹ��ṩ�ĸ߼���ѯ���ԣ��������ܹ�֧���Ӳ�ѯ��
<br>
- �߼�����
JPA �ܹ�֧���������ĸ߼����ԣ�������֮��ļ̳С���̬�ȸ��ӹ�ϵ��������֧���ܹ��ÿ���������޶ȵ�ʹ����������ģ�������ҵӦ�ã�������Ҫ���д�����Щ�����ڹ�ϵ���ݿ�ĳ־û���

# 3. JPA ������
## 3-1. ���Ŀ����
������Ҫ����һ�����̣����漰ҳ�潻�������Դ���һ���򵥵� Maven ���̼��ɡ�
### 3-1-1. �������
```xml
<properties>
    <project.hibernate.version>5.0.7.Final</project.hibernate.version>
</properties>

<dependencies>
    <!--junit-->
    <dependency>
        <groupId>junit</groupId>
        <artifactId>junit</artifactId>
        <version>4.12</version>
        <scope>test</scope>
    </dependency>
    
    <!--hibernate��jpa��֧��-->
    <dependency>
        <groupId>org.hibernate</groupId>
        <artifactId>hibernate-entitymanager</artifactId>
        <version>${project.hibernate.version}</version>
    </dependency>
    
    <!--c3p0-->
    <dependency>
        <groupId>org.hibernate</groupId>
        <artifactId>hibernate-c3p0</artifactId>
        <version>${project.hibernate.version}</version>
    </dependency>
    
    <!--log4j-->
    <dependency>
        <groupId>log4j</groupId>
        <artifactId>log4j</artifactId>
        <version>1.2.17</version>
    </dependency>
    
    <!--mysql-->
    <dependency>
        <groupId>mysql</groupId>
        <artifactId>mysql-connector-java</artifactId>
        <version>5.1.45</version>
    </dependency>
</dependencies>
```

### 3-1-2. ��д JPA ����
JPA �������ļ����������Ŀ resource Ŀ¼�µ� META-INF �ļ����£������Ʊ���Ϊ persistence.xml

```xml
<?xml version="1.0" encoding="UTF-8"?>
<persistence xmlns="http://java.sun.com/xml/ns/persistence" version="2.0">
    <!--
        �־û���Ԫ
            name: ��Ԫ����
            transaction-type: �������ʽ
                JTA: �ֲ�ʽ�������
                RESOURCE_LOCAL: �����������
    -->
    <persistence-unit name="myJpa" transaction-type="RESOURCE_LOCAL">
        <!--JPA��ʵ��-->
        <provider>org.hibernate.jpa.HibernatePersistenceProvider</provider>

        <!--��ѡ���ã�JPA��ʵ�����ã�����Hibernate�����ã�-->
        <properties>
            <!--���ݿ�����-->
            <property name="javax.persistence.jdbc.user" value="root"/>
            <property name="javax.persistence.jdbc.password" value="root"/>
            <property name="javax.persistence.jdbc.driver" value="com.mysql.jdbc.Driver"/>
            <property name="javax.persistence.jdbc.url" value="jdbc:mysql://localhost:3306/test"/>
            
            <!--Hibernate����-->
            <property name="hibernate.show_sql" value="true"/> <!--��ʾSQL��true/false��-->
            <property name="hibernate.hbm2ddl.auto" value="update"/><!--�Զ�������create/update/none��-->
        </properties>
    </persistence-unit>
</persistence>
```

### 3-1-3. ��дʵ����
ʹ�� JDK5.0 ע��������ʵ��������ݿ���ӳ���ϵ
```java
/**
 * �ͻ���ʵ����
 * @author qinghua
 * @date 2018/9/7 21:16
 */
@Entity //����ʵ����
@Table(name = "cst_customer") //ʵ����ͱ��ӳ���ϵ
public class Customer {

    /**
     * �������ɲ���
     * IDENTITY: ��Ҫ���ݿ�֧���Զ����� (MySQL,SqlServer)
     * SEQUENCE: ��Ҫ���ݿ�֧������ (Oracle)
     * TABLE : ��JPAά��һ�Ŷ�����������
     * AUTO : �������ݿ������Զ�ѡ�����ɲ���
     */
    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    @Column(name = "cust_id")
    private Long custId; //�ͻ���ţ�������
    @Column(name = "cust_name")
    private String custName; //�ͻ����ƣ���˾���ƣ�
    @Column(name = "cust_source")
    private String custSource; //�ͻ���Ϣ��Դ
    @Column(name = "cust_industry")
    private String custIndustry;//�ͻ�������ҵ
    @Column(name = "cust_level")
    private String custLevel; //�ͻ�����
    @Column(name = "cust_address")
    private String custAddress; //�ͻ���ϵ��ַ
    @Column(name = "cust_phone")
    private String custPhone; //�ͻ���ϵ�绰
    
    //ʡ�� getter & setter

    //ʡ�� toString()
}
```

## 3-2. ��һ�� JPA ����
- JPA �Ļ�����ɾ�Ĳ�һ��6������
    - ���������ļ�������ʵ�����������
    - ��ʵ������������л��ʵ�������
    - ��ʵ��������л���������
    - ʹ��ʵ���������� CRUD ����
    - �ύ��ع�����
    - �ͷ���Դ
<br>
- ����Ĵ�����һ���򵥵ı������
    ```java
    @Test
    public void testSave() {
        //1�����������ļ�������ʵ�����������
        EntityManagerFactory factory = Persistence.createEntityManagerFactory("myJpa");
    
        //2����ʵ������������л��ʵ�������
        EntityManager manager = factory.createEntityManager();
    
        //3����ʵ��������л���������
        EntityTransaction transaction = manager.getTransaction();
        transaction.begin();
    
        //4��ʹ��ʵ���������� CRUD ����
        Customer customer = new Customer();
        customer.setCustName("Google");
        customer.setCustIndustry("������");

        manager.persist(customer); //�������

        //5���ύ��ع�����
        transaction.commit();
    
        //6���ͷ���Դ
        manager.close();
        factory.close();
    }
    ```
<br>
- ʵ�����������������
������Ĵ����п��Կ�����ʵ�������������ÿ�����Է�������Ҫ�ظ��Ĵ������ӹ����л�õ�ʵ���������ʹ����Ϻ���Ҫ�ͷţ�������˲���Ҫ��ʱ�俪�������Ա�дһ��ʵ������������Ĺ����࣬�ڹ�������ά��һ��ʵ�����������������Ӧ��ֻ����һ���������ṩһ���������ʵ���������ʹ����Ϻ�Ҳ�����ͷ���Դ��
    ```java
    /**
     * ʵ�������������
     *
     * @author qinghua
     * @date 2018/9/12 12:26
     */
    public class JpaUtils {
    
        /**
         * ά��һ��������ʵ�������������
         */
        private static EntityManagerFactory factory;
    
        /**
         * �ھ�̬������м��������ļ�����ʼ������������
         */
        static {
            factory = Persistence.createEntityManagerFactory("myJpa");
        }
    
        /**
         * �ӹ����л�ȡһ��ʵ�������
         * @return
         */
        public static EntityManager getEntityManager() {
            return factory.createEntityManager();
        }
    }
    ```

## 3-3. ��ɾ�Ĳ�
JPA ��ʵ��������ṩ�˻�������ɾ�Ĳ� API
| ���� | ���� |
| --- |
| ���� | `persist`(T entity) |
| ��ѯ���������أ� | `find`(Class entityClass, Long primaryKey) |
| ��ѯ���ӳټ��أ� | `getReference`(Class entityClass, Long primaryKey) |
| ���� | `merge`(T entity) |
| ɾ�� | `remove`(T entity) |
<br>
����ʾ����
```java
package com.example.test;

import com.example.domain.Customer;
import com.example.entity.JpaUtils;
import org.junit.Test;

import javax.persistence.EntityManager;
import javax.persistence.EntityTransaction;

/**
 * @author qinghua
 * @date 2018/9/7 21:27
 */
public class JpaTest {

    /**
     * ����, persist
     */
    @Test
    public void testSave() {

        //�ӹ������л��ʵ�������
        EntityManager manager = JpaUtils.getEntityManager();

        //��ȡ������󣬿�������
        EntityTransaction transaction = manager.getTransaction();
        transaction.begin();

        //�����ɾ�Ĳ����
        Customer customer = new Customer();
        customer.setCustName("Google");
        customer.setCustIndustry("������");

        //�ύ��ع�����
        manager.persist(customer); //�������
        transaction.commit();
    }

    /**
     * ����������ѯ����ʱ���أ�,find
     */
    @Test
    public void testFind() {
        //ͨ����������ʵ�������
        EntityManager entityManager = JpaUtils.getEntityManager();

        /**
         * ִ�в�ѯ
         *
         * ����һ��Class���ֽ��룩����ָ��ѯ�������ݷ�װ�������ʵ�������
         * ������������
         */
        Customer customer = entityManager.find(Customer.class, 1L);
        System.out.println(customer);
    }

    /**
     * ����������ѯ���ӳټ��أ�,getReference
     */
    @Test
    public void testGetReference() {
        //ͨ����������ʵ�������
        EntityManager entityManager = JpaUtils.getEntityManager();

        /**
         * ִ�в�ѯ
         *
         * ����һ��Class���ֽ��룩����ָ��ѯ�������ݷ�װ�������ʵ�������
         * ������������
         */
        Customer customer = entityManager.getReference(Customer.class, 1L);
        System.out.println(customer);
    }

    /**
     * ɾ����¼, remove
     */
    @Test
    public void testRemove() {
        //ͨ����������ʵ�������
        EntityManager entityManager = JpaUtils.getEntityManager();

        //��������
        EntityTransaction transaction = entityManager.getTransaction();
        transaction.begin();

        //�Ȳ�ѯ��Ҫɾ���ļ�¼
        Customer customer = entityManager.find(Customer.class, 1L);

        //ִ��ɾ��
        entityManager.remove(customer);

        //�ύ����
        transaction.commit();
    }

    /**
     * ���¼�¼, merge
     */
    @Test
    public void testUpdate() {
        //ͨ����������ʵ�������
        EntityManager entityManager = JpaUtils.getEntityManager();

        //��������
        EntityTransaction transaction = entityManager.getTransaction();
        transaction.begin();

        //�Ȳ�ѯ��Ҫɾ���ļ�¼
        Customer customer = entityManager.find(Customer.class, 1L);
        customer.setCustPhone("13800138000");

        //ִ�и���
        entityManager.merge(customer);

        //�ύ����
        transaction.commit();
    }
}
```

## 3-4. JPQL ��ѯ
&emsp;&emsp;JPQL��Java Persistence Query Language���� JPA �ƶ����������Ĳ�ѯ���ԣ���Ŀ����Ϊ�˱��������SQL ������ϣ��﷨�� SQL �ǳ����ƣ���ͬ���� SQL ����������ݿ����ֶΣ��� JPQL �������ʵ��������ԡ�
<br>
SQL �� JPQL ���﷨���죺
| ���� | �﷨ʾ�� |
| --- |
| SQL | select * from ���� where �ֶ��� = ? and �ֶ��� = ? |
| JPQL | from ���� where ������ = ? and ������ = ? |
<br>
&emsp;&emsp;JPQL ��ѯ��Ҫͨ��ʵ���������EntityManager���� createQuery(String jpql) ��������һ�� JPQL ���������һ�� Query ������ͨ�� Query ����ķ������в�����ֵ��ִ�в�ѯ������������һЩ�򵥵�ʾ������
```java
package com.example.test;

import com.example.domain.Customer;
import com.example.entity.JpaUtils;
import org.junit.Test;

import javax.persistence.EntityManager;
import javax.persistence.Query;
import java.util.List;

/**
 * @author qinghua
 * @date 2018/9/14 16:50
 */
public class JpqlTest {

    /**
     * ��ѯ����
     */
    @Test
    public void testFindAll() {
        //���ʵ�������
        EntityManager entityManager = JpaUtils.getEntityManager();

        //����Query����
        String jpql = "from Customer";
        Query query = entityManager.createQuery(jpql);

        //ִ�в�ѯ
        List<Customer> list = query.getResultList();
        
        //����
        for (Customer customer : list) {
            System.out.println(customer);
        }
    }

    /**
     * ����
     */
    @Test
    public void testOrderBy() {
        //���ʵ�������
        EntityManager entityManager = JpaUtils.getEntityManager();

        //����Query����
        String jpql = "from Customer order by custId desc";
        Query query = entityManager.createQuery(jpql);

        //ִ�в�ѯ
        List<Customer> list = query.getResultList();
        
        //����
        for (Customer customer : list) {
            System.out.println(customer);
        }
    }

    /**
     * ͳ�Ʋ�ѯ
     */
    @Test
    public void testCount() {
        //���ʵ�������
        EntityManager entityManager = JpaUtils.getEntityManager();

        //����Query����
        String jpql = "select count(custId) from Customer";
        Query query = entityManager.createQuery(jpql);
        
        //ִ�в�ѯ
        Object count = query.getSingleResult();

        System.out.println(count);
    }

    /**
     * ��ҳ
     */
    @Test
    public void testFindPage() {
        //���ʵ�������
        EntityManager entityManager = JpaUtils.getEntityManager();

        //����Query����
        String jpql = "from Customer";
        Query query = entityManager.createQuery(jpql);

        //���÷�ҳ����
        query.setFirstResult(1);
        query.setMaxResults(2);

        //ִ�в�ѯ
        List<Customer> list = query.getResultList();
        
        //����
        for (Customer customer : list) {
            System.out.println(customer);
        }
    }

    /**
     * ������ѯ
     */
    @Test
    public void testLike() {
        //���ʵ�������
        EntityManager entityManager = JpaUtils.getEntityManager();

        //����Query����
        String jpql = "from Customer where custName like ?1";
        Query query = entityManager.createQuery(jpql);

        //���ò���
        query.setParameter(1, "G%");

        //ִ�в�ѯ
        List<Customer> list = query.getResultList();
        
        //����
        for (Customer customer : list) {
            System.out.println(customer);
        }
    }
}
```

# 4. Spring Data JPA
&emsp;&emsp; Spring Data JPA �Ļ��������ڱ��ĵ�ǰ�Բ����Ѿ����˽��ܣ����ﲻ���ظ���
## 4-1. ���Ŀ����
### 4-1-1. ��������
����һ���� Maven ��Ŀ��

### 4-1-2. �������
```xml
<properties>
    <spring.version>5.0.2.RELEASE</spring.version>
    <hibernate.version>5.0.7.Final</hibernate.version>
    <slf4j.version>1.6.6</slf4j.version>
    <log4j.version>1.2.12</log4j.version>
    <c3p0.version>0.9.1.2</c3p0.version>
    <mysql.version>5.1.6</mysql.version>
</properties>

<dependencies>
    <!--junit-->
    <dependency>
        <groupId>junit</groupId>
        <artifactId>junit</artifactId>
        <version>4.12</version>
        <scope>test</scope>
    </dependency>

    <!--spring-->
    <dependency>
        <groupId>org.aspectj</groupId>
        <artifactId>aspectjweaver</artifactId>
        <version>1.8.13</version>
    </dependency>
    <dependency>
        <groupId>org.springframework</groupId>
        <artifactId>spring-aop</artifactId>
        <version>${spring.version}</version>
    </dependency>
    <dependency>
        <groupId>org.springframework</groupId>
        <artifactId>spring-context-support</artifactId>
        <version>${spring.version}</version>
    </dependency>
    <dependency>
        <groupId>org.springframework</groupId>
        <artifactId>spring-orm</artifactId>
        <version>${spring.version}</version>
    </dependency>
    <dependency>
        <groupId>org.springframework</groupId>
        <artifactId>spring-test</artifactId>
        <version>${spring.version}</version>
    </dependency>

    <!--spring data jpa-->
    <dependency>
        <groupId>org.springframework.data</groupId>
        <artifactId>spring-data-jpa</artifactId>
        <version>2.0.5.RELEASE</version>
    </dependency>

    <!--el(spring data jpa ����el)-->
    <dependency>
        <groupId>org.glassfish.web</groupId>
        <artifactId>javax.el</artifactId>
        <version>2.2.4</version>
    </dependency>

    <!--hibernate-->
    <dependency><!--hibernate jpa ʵ��-->
        <groupId>org.hibernate</groupId>
        <artifactId>hibernate-entitymanager</artifactId>
        <version>${hibernate.version}</version>
    </dependency>
    <dependency><!--hibernate У��-->
        <groupId>org.hibernate</groupId>
        <artifactId>hibernate-validator</artifactId>
        <version>5.2.1.Final</version>
    </dependency>

    <!--c3-0-->
    <dependency>
        <groupId>c3p0</groupId>
        <artifactId>c3p0</artifactId>
        <version>${c3p0.version}</version>
    </dependency>

    <!--log-->
    <dependency>
        <groupId>log4j</groupId>
        <artifactId>log4j</artifactId>
        <version>${log4j.version}</version>
    </dependency>
    <dependency>
        <groupId>org.slf4j</groupId>
        <artifactId>slf4j-log4j12</artifactId>
        <version>${slf4j.version}</version>
    </dependency>

    <!--mysql-->
    <dependency>
        <groupId>mysql</groupId>
        <artifactId>mysql-connector-java</artifactId>
        <version>${mysql.version}</version>
    </dependency>

</dependencies>
```

### 4-1-3. ��д Spring ����
Spring Data JPA �������ļ�����Spring�������ļ�
```xml
<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
    xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    xmlns:aop="http://www.springframework.org/schema/aop"
    xmlns:context="http://www.springframework.org/schema/context"
    xmlns:tx="http://www.springframework.org/schema/tx"
    xmlns:jpa="http://www.springframework.org/schema/data/jpa"
    xsi:schemaLocation="
        http://www.springframework.org/schema/beans
        http://www.springframework.org/schema/beans/spring-beans.xsd
        http://www.springframework.org/schema/aop
        http://www.springframework.org/schema/aop/spring-aop.xsd
        http://www.springframework.org/schema/context
        http://www.springframework.org/schema/context/spring-context.xsd
        http://www.springframework.org/schema/tx
        http://www.springframework.org/schema/tx/spring-tx.xsd
        http://www.springframework.org/schema/data/jpa
        http://www.springframework.org/schema/data/jpa/spring-jpa.xsd">

    <!--ʵ�������-->
    <bean id="entityManagerFactory" class="org.springframework.orm.jpa.LocalContainerEntityManagerFactoryBean">
        <property name="dataSource" ref="dataSource"/><!--���ӳ�-->
        <property name="packagesToScan" value="com.example.domain"/><!--ʵ�������ڵİ�-->
        <property name="persistenceProvider"><!--jpa ʵ���ṩ��-->
            <bean class="org.hibernate.jpa.HibernatePersistenceProvider"/>
        </property>
        <property name="jpaVendorAdapter"><!--jpa �ṩ������-->
            <bean class="org.springframework.orm.jpa.vendor.HibernateJpaVendorAdapter">
                <property name="generateDdl" value="false"/><!--�Զ��������ݿ��-->
                <property name="database" value="MYSQL"/><!--���ݿ�����-->
                <property name="databasePlatform" value="org.hibernate.dialect.MySQLDialect"/><!--���ݿⷽ��-->
                <property name="showSql" value="true"/><!--��ʾSQL���-->
            </bean>
        </property>
        <property name="jpaDialect"><!--jpa ���ԣ�hibernate�߼����ԣ�-->
            <bean class="org.springframework.orm.jpa.vendor.HibernateJpaDialect"/>
        </property>
    </bean>

    <!--���ӳ�-->
    <bean id="dataSource" class="com.mchange.v2.c3p0.ComboPooledDataSource">
        <property name="driverClass" value="com.mysql.jdbc.Driver"/>
        <property name="jdbcUrl" value="jdbc:mysql://localhost:3306/test"/>
        <property name="user" value="root"/>
        <property name="password" value="root"/>
    </bean>

    <!--spring data jpa ����-->
    <jpa:repositories
            base-package="com.example.repository"
            repository-impl-postfix="Impl"
            entity-manager-factory-ref="entityManagerFactory"
            transaction-manager-ref="jpaTransactionManager"/>

    <!--���������-->
    <bean id="jpaTransactionManager" class="org.springframework.orm.jpa.JpaTransactionManager">
        <property name="entityManagerFactory" ref="entityManagerFactory"/><!--ʵ�������-->
    </bean>

    <!--ע������-->
    <tx:annotation-driven transaction-manager="jpaTransactionManager" proxy-target-class="true"/>

</beans>
```

### 4-1-4. ��д�־ò�ӿ�
Ҫʹ�� Spring Data JPA������������Ĺ淶���־ò�ӿ���Ҫ�̳� JpaRepository �ӿڡ�
`CustomerRepository.java`
```java
/**
 * @author qinghua
 * @date 2018/9/15 14:54
 *
 * JpaRepository<ʵ������, ʵ������������> Ҫ����JPA�淶,����̳�JpaRepository
 * JpaSpecificationExecutor<ʵ������> JPA�ṩ�ĵ���̬��ѯ�ӿ�
 */
public interface CustomerRepository extends JpaRepository<Customer, Long>, JpaSpecificationExecutor<Customer> {
    //...
}
```

## 4-2. ��ɾ�Ĳ�
```java
package com.example;

import com.example.domain.Customer;
import com.example.repository.CustomerRepository;
import org.junit.Test;
import org.junit.runner.RunWith;
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.test.context.ContextConfiguration;
import org.springframework.test.context.junit4.SpringJUnit4ClassRunner;

import java.util.List;

/**
 * @author qinghua
 * @date 2018/9/15 14:54
 */
@RunWith(SpringJUnit4ClassRunner.class)
@ContextConfiguration(locations = "classpath:applicationContext.xml")
public class CustomerRepositoryTest {

    @Autowired
    private CustomerRepository customerRepository;

    /**
     * ����ID��ѯ
     */
    @Test
    public void testFindById() {
        Customer customer = customerRepository.findById(1L).get();
        System.out.println(customer);
    }

    /**
     * ����/���¶���
     * ���ݵĶ��������ID��ֱ�ӱ���
     * ���ݵĶ������û��ID���Ȳ�ѯID�Ƿ���ڣ�����������޸ģ��������򱣴�
     */
    @Test
    public void testSave() {
        //����Ҫ����Ķ���
        Customer customer = new Customer();
        customer.setCustId(6L);
        customer.setCustName("Facebook");
        customer.setCustIndustry("IT/������");

        //ִ�б������²���
        Customer dbCustomer = customerRepository.save(customer);
        System.out.println(dbCustomer);
    }

    /**
     * ����IDɾ��
     */
    @Test
    public void testDeleteById() {
        customerRepository.deleteById(6L);
    }

    /**
     * ��ѯ���пͻ�
     */
    @Test
    public void testFindAll() {
        List<Customer> list = customerRepository.findAll();
        for (Customer customer : list) {
            System.out.println(customer);
        }
    }

}
```

## 4-3. ������ѯ
JPA ���˻�������ɾ�Ĳ����⣬��֧�ֲ�ѯ������`count`�����ж������Ƿ���ڣ�`exists`�����ӳټ��أ�`getById`���ȡ�
ʾ������
```java
package com.example;

import com.example.domain.Customer;
import com.example.repository.CustomerRepository;
import org.junit.Test;
import org.junit.runner.RunWith;
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.test.context.ContextConfiguration;
import org.springframework.test.context.junit4.SpringJUnit4ClassRunner;

import java.util.List;

/**
 * @author qinghua
 * @date 2018/9/15 14:54
 */
@RunWith(SpringJUnit4ClassRunner.class)
@ContextConfiguration(locations = "classpath:applicationContext.xml")
public class CustomerRepositoryTest {

    @Autowired
    private CustomerRepository customerRepository;

    /**
     * ��ѯ����
     */
    @Test
    public void testCount() {
        long count = customerRepository.count();
        System.out.println(count);
    }

    /**
     * ����ID�жϼ�¼�Ƿ����
     */
    @Test
    public void testExistsById() {
        boolean exists = customerRepository.existsById(3L);
        System.out.println(exists);
    }

    /**
     * �ӳټ���
     * �ײ���õ��� em.getReference
     */
    @Test
    public void testGetOne() {
        Customer customer = customerRepository.getOne(1L);
        System.out.println(customer);
    }

}
```

## 4-4. JPQL �� ���� SQL
### 4-4-1. JPQL ��ѯ
Spring Data JPA ֧�� JPQL ��ѯ�������Ҫʹ�� JPQL ��Ҫ�ڳ־ò�ӿ��ж�����󷽷������ڳ��󷽷���ʹ�� `@Query` ע�⡣
<br>
- JPQL ��ѯ
�ڳ־ò�ӿڶ�����󷽷�������� JPQL �������ݿ�����Ĵ���ע�ͣ�
    ```java
    /**
     * @author qinghua
     * @date 2018/9/15 14:54
     */
    public interface CustomerRepository extends JpaRepository<Customer, Long> {
    
        /**
         * �������ƺ�ID��ѯ�ͻ�
         *
         * �滻ռλ��ע�⣺
         * JPQL ����е�ռλ��Ĭ�ϰ��βε�˳������滻
         * �����Ҫ����˳��ֻ��Ҫ��ռλ����������βε�����ֵ
         *
         * @param name
         * @return
         */
        @Query(value = "from Customer where custName = ?1 and custId = ?2")
        Customer findByName(String name, Long id);
    }
    ```
<br>
- JPQL �޸�
JPQL ����֧�ֲ�ѯ��Ҳ֧�����ݿ�ĸ��º�ɾ���������� Spring Data JPA ��Ҫʹ�� JPQL ���޸ĺ�ɾ���������־ò�ӿڵķ����ϲ�����Ҫ��� `@Query` ����������Ҫ���һ�� `@Modifiy` ��ǩ
<br>
ʾ�����룺
    ```java
    /**
     * @author qinghua
     * @date 2018/9/15 14:54
     */
    public interface CustomerRepository extends JpaRepository<Customer, Long> {
    
        /**
         * ����ID�޸Ŀͻ�������
         * @param name
         * @param id
         */
        @Query(value = "update Customer set custName = ?1 where custId = ?2")
        @Modifying //��ʾ����һ���޸Ĳ���������Ҫ�ӣ�
        void updateCustomer(String name, Long id);

    }
    ```
�־ò�ӿڵķ���д���ˣ���ʱ����ڲ��Է�����ִ���޸ģ����ݿ��еļ�¼�����ᷢ���仯�����Ҫʹ�� JPQL �����޸ĺ�ɾ��������ִ�еĲ�������Ҫ��������ƣ��������ύ����
<br>
����ʾ�����룺
    ```java
    /**
     * @author qinghua
     * @date 2018/9/15 16:12
     */
    @RunWith(SpringJUnit4ClassRunner.class)
    @ContextConfiguration(locations = "classpath:applicationContext.xml")
    public class JPQLTest {

        @Autowired
        private CustomerRepository customerRepository;
        
        /**
         * JPQL �޸�
         */
        @Test
        @Transactional //�������
        @Commit //�ύ����
        public void testUpdate() {
            customerRepository.updateCustomer("IBM", 5L);
        }

    }
    ```

### 4-4-2. ���� SQL ��ѯ
Spring Data JPA ͬʱҲ֧��ʹ��ԭ���� SQL ���в�ѯ��ֻ��Ҫ�� `@Query` ע��� `nativeQuery` ��������Ϊ true ���ɡ�
<br>
ʾ������
```java
/**
 * @author qinghua
 * @date 2018/9/15 14:54
 */
public interface CustomerRepository extends JpaRepository<Customer, Long> {

    /**
     * ʹ�ñ���SQL��ѯ
     *
     * Queryע��
     * value ��JPQL��� / SQL���
     * nativeQuery ���Ƿ�ʹ�ñ���SQL��ѯ��Ϊtrueʱ��value�е�ֵ���ᱻ��Ϊ����SQL���ִ��
     *
     * ��ʱ����ֵ��List<Object[]>��Ҳ����ӳ��Ϊʵ�������ļ���List<Customer>
     *
     * @param name
     * @return
     */
    @Query(value = "select * from cst_customer where cust_name like ?1", nativeQuery = true)
    List<Object[]> findByName(String name);

}
```

# 5. ����������ѯ
Spring Data JPA �ܸ��ݷ��������ֶ�̬���� SQL ��䣬ֻ��Ҫ���� Spring Data JPA ��������Ĺ��������巽�����ɡ�<br/>
<br>
## 5-1. ����������ѯ�Ĺ���
| Keyword | Sample | JPQL snippet |
| --- |
| And | findByLastnameAndFirstname | �� where x.lastname = ?1 and x.firstname = ?2 |
| Or | findByLastnameOrFirstname | �� where x.lastname = ?1 or x.firstname = ?2 |
| Is,Equals | findByFirstname,findByFirstnameIs,findByFirstnameEquals | �� where x.firstname = ?1 |
| Between | findByStartDateBetween | �� where x.startDate between ?1 and ?2 |
| LessThan | findByAgeLessThan | �� where x.age < ?1 |
| LessThanEqual | findByAgeLessThanEqual | �� where x.age <= ?1 |
| GreaterThan | findByAgeGreaterThan | �� where x.age > ?1 |
| GreaterThanEqual | findByAgeGreaterThanEqual | �� where x.age >= ?1 |
| After | findByStartDateAfter | �� where x.startDate > ?1 |
| Before | findByStartDateBefore | �� where x.startDate < ?1 |
| IsNull | findByAgeIsNull | �� where x.age is null |
| IsNotNull,NotNull | findByAge(Is)NotNull | �� where x.age not null |
| Like | findByFirstnameLike | �� where x.firstname like ?1 |
| NotLike | findByFirstnameNotLike | �� where x.firstname not like ?1 |
| StartingWith | findByFirstnameStartingWith | �� where x.firstname like ?1(parameter bound with appended %) |
| EndingWith | findByFirstnameEndingWith | �� where x.firstname like ?1(parameter bound with prepended %) |
| Containing | findByFirstnameContaining | �� where x.firstname like ?1(parameter bound wrapped in %) |
| OrderBy | findByAgeOrderByLastnameDesc | �� where x.age = ?1 order by x.lastname desc |
| Not | findByLastnameNot | �� where x.lastname <> ?1 |
| In | findByAgeIn(Collection<Age> ages) | �� where x.age in ?1 |
| NotIn | findByAgeNotIn(Collection<Age> ages) | �� where x.age not in ?1 |
| TRUE | findByActiveTrue() | �� where x.active = true |
| FALSE | findByActiveFalse() | �� where x.active = false |
| IgnoreCase | findByFirstnameIgnoreCase | �� where UPPER(x.firstame) = UPPER(?1) |

## 5-2. ��������ʾ��
```java
/**
 * @author qinghua
 * @date 2018/9/15 14:54
 */
public interface CustomerRepository extends JpaRepository<Customer, Long> {

    /**
     * And
     * �� where x.cust_name = ?1 and x.cust_industry = ?2
     */
    List<Customer> findByCustNameAndCustIndustry(String custName, String industry);

    /**
     * Or
     * �� where x.cust_name = ?1 or x.cust_industry = ?2
     */
    List<Customer> findByCustNameOrCustIndustry(String custName, String industry);

    /**
     * is | equals
     * �� where x.cust_name = ?1
     */
    List<Customer> findByCustNameEquals(String custName);

    /**
     * Between
     * �� where x.cust_id between ?1 and ?2
     */
    List<Customer> findByCustIdBetween(Long start, Long end);

    /**
     * LessThan
     * �� where x.cust_id < ?1
     */
    List<Customer> findByCustIdLessThan(Long custId);

    /**
     * LessThanEqual
     * �� where x.cust_id <= ?1
     */
    List<Customer> findByCustIdLessThanEqual(Long custId);

    /**
     * GreaterThan
     * �� where x.cust_id > ?1
     */
    List<Customer> findByCustIdGreaterThan(Long custId);

    /**
     * GreaterThanEqual
     * �� where x.cust_id >= ?1
     */
    List<Customer> findByCustIdGreaterThanEqual(Long custId);

    /**
     * After
     * �� where x.cust_id > ?1
     */
    List<Customer> findByCustIdAfter(Long custId);

    /**
     * Before
     * �� where x.cust_id < ?1
     */
    List<Customer> findByCustIdBefore(Long custId);

    /**
     * IsNull
     * �� where x.cust_phone is null
     */
    List<Customer> findByCustPhoneIsNull();

    /**
     * Before
     * �� where x.cust_phone is not null
     */
    List<Customer> findByCustPhoneIsNotNull();

    /**
     * Like
     * �� where x.cust_name like ?1
     */
    List<Customer> findByCustNameLike(String custName);

    /**
     * NotLike
     * �� where x.cust_name not like ?1
     */
    List<Customer> findByCustNameNotLike(String custName);

    /**
     * NotLike
     * �� where x.cust_name like %?1
     */
    List<Customer> findByCustNameStartingWith(String custName);

    /**
     * NotLike
     * �� where x.cust_name like ?1%
     */
    List<Customer> findByCustNameEndingWith(String custName);

    /**
     * NotLike
     * �� where x.cust_name like %?1%
     */
    List<Customer> findByCustNameContaining(String custName);

    /**
     * OrderBy
     * �� where x.cust_name like %?1% order by cust_id desc
     */
    List<Customer> findByCustNameContainingOrderByCustIdDesc(String custName);

    /**
     * Not
     * �� where x.cust_name != ?1
     */
    List<Customer> findByCustNameNot(String custName);

    /**
     * In
     * �� where x.cust_id in (ids)
     */
    List<Customer> findByCustIdIn(List<Long> ids);

    /**
     * NotIn
     * �� where x.cust_id not in (ids)
     */
    List<Customer> findByCustIdNotIn(List<Long> ids);

}
```

# 6. Specifications ��̬��ѯ
## 6-1. ��̬��ѯ�ķ����б�
`JpaSpecificationExecutor`
```java
/**
 * ��ѯһ������
 */
Optional<T> findOne(@Nullable Specification<T> spec);

/**
 * ��ѯ�������
 */
List<T> findAll(@Nullable Specification<T> spec);

/**
 * ��ҳ��ѯ
 */
Page<T> findAll(@Nullable Specification<T> spec, Pageable pageable);

/**
 * �����ѯ
 */
List<T> findAll(@Nullable Specification<T> spec, Sort sort);

/**
 * ͳ�Ʋ�ѯ
 */
long count(@Nullable Specification<T> spec);
```

## 6-2. ������ѯ����
### 6-2-1. �־ò�ӿ�׼��
Ҫʹ��Specification������ѯ���־ò�ӿڱ���̳�JpaSpecification�ӿڡ�
`CustomerRepository`
```java
/**
 * @author qinghua
 * @date 2018/9/21 10:46
 */
public interface CustomerRepository extends JpaRepository<Customer, Long>, JpaSpecificationExecutor<Customer> {

}
```

### 6-2-2. ������ѯʾ��
```java
/**
 * @author qinghua
 * @date 2018/9/21 10:47
 */
@RunWith(SpringJUnit4ClassRunner.class)
@ContextConfiguration(locations = {"classpath:applicationContext.xml"})
public class SpecificationTest {

    @Autowired
    private CustomerRepository customerRepository;

    /**
     * ��������׼ƥ�䣬��ѯһ���ͻ�
     */
    @Test
    public void testFindOne() {
        Customer customer = customerRepository.findOne(new Specification<Customer>() {

            /**
             *
             * @param root ��ȡҪ��ѯ�Ķ�������
             * @param query ������ѯ����
             * @param criteriaBuilder ����������
             * @return
             */
            @Override
            public Predicate toPredicate(Root<Customer> root, CriteriaQuery<?> query, CriteriaBuilder criteriaBuilder) {
                //����Ϊ���������Թ�����·������
                Path<Object> custName = root.get("custName");

                //������׼ƥ��Ķ��Զ���
                Predicate predicate = criteriaBuilder.equal(custName, "Google");

                return predicate;
            }
        }).get();

        System.out.println(customer);
    }

    /**
     * ��������׼ƥ�䣬��ѯһ���ͻ�
     */
    @Test
    public void testFindOne2() {
        Customer customer = customerRepository.findOne(new Specification<Customer>() {
            @Override
            public Predicate toPredicate(Root<Customer> root, CriteriaQuery<?> query, CriteriaBuilder criteriaBuilder) {
                //����Ϊ���������Թ�����·������
                Path<Object> custName = root.get("custName");
                Path<Object> custIndustry = root.get("custIndustry");

                //������׼ƥ��Ķ��Զ���
                Predicate p1 = criteriaBuilder.equal(custName, "Google");
                Predicate p2 = criteriaBuilder.equal(custIndustry, "������");

                //��������׼ƥ�佨��And��ϵ
                Predicate predicate = criteriaBuilder.and(p1, p2);

                return predicate;
            }
        }).get();

        System.out.println(customer);
    }

    /**
     * ģ��ƥ�䣬��ѯ�ͻ��б�
     */
    @Test
    public void testFindAll() {
        List<Customer> list = customerRepository.findAll(new Specification<Customer>() {
            @Override
            public Predicate toPredicate(Root<Customer> root, CriteriaQuery<?> query, CriteriaBuilder criteriaBuilder) {
                //����Ϊ���������Թ�����·������
                Path<Object> custName = root.get("custName");

                //���� gt,lt,ge,le,like ��ѯ����Ҫ����·������ָ����������������������
                Predicate predicate = criteriaBuilder.like(custName.as(String.class), "%o%");
                return predicate;
            }
        });

        for (Customer customer : list) {
            System.out.println(customer);
        }
    }

    /**
     * �����ѯ
     * Sort.by(�������, ��������)
     */
    @Test
    public void testSort() {
        List<Customer> list = customerRepository.findAll(new Specification<Customer>() {
            @Override
            public Predicate toPredicate(Root<Customer> root, CriteriaQuery<?> query, CriteriaBuilder criteriaBuilder) {
                //�����ﹹ����ѯ����������null��ʾû��������ѯ����
                return null;
            }
        }, Sort.by(Sort.Direction.DESC, "custId"));

        for (Customer customer : list) {
            System.out.println(customer);
        }
    }

    /**
     * ��ҳ��ѯ
     * Spring4.x �ķ�ҳ������ new PageRequest(page, size)
     * Spring5.x ��ʹ��PageRequest.of(page, size)
     */
    @Test
    public void testPageable() {
        Page<Customer> page = customerRepository.findAll(new Specification<Customer>() {
            @Override
            public Predicate toPredicate(Root<Customer> root, CriteriaQuery<?> query, CriteriaBuilder criteriaBuilder) {
                //�����ﹹ����ѯ����������null��ʾû��������ѯ����
                return null;
            }
        }, PageRequest.of(1, 3)); //pageҳ���0��ʼ

        System.out.println("TotalElements:" + page.getTotalElements());//�ܼ�¼��
        System.out.println("TotalPages:" + page.getTotalPages());//��ҳ��
        System.out.println("Size:" + page.getSize());//ÿҳ��ʾ�ļ�¼��

        List<Customer> list = page.getContent();
        for (Customer customer : list) {
            System.out.println(customer);
        }
    }


    /**
     * ��ѯ����
     */
    @Test
    public void testCount() {
        long count = customerRepository.count(new Specification<Customer>() {
            @Override
            public Predicate toPredicate(Root<Customer> root, CriteriaQuery<?> query, CriteriaBuilder criteriaBuilder) {
                Path<Object> custName = root.get("custName");
                Predicate predicate = criteriaBuilder.like(custName.as(String.class), "%o%");
                return predicate;
            }
        });

        System.out.println(count);
    }
}
```
# 7. ���Ĺ�ϵ�Ͳ���
## 7-1. һ�Զ�
### 7-1-1. ��ȷ���ϵ
- **�ͻ���**
һ�ҹ�˾��Google��˾����˾�Ŀͻ���˾��
- **��ϵ�˱�**
��ҹ�˾����ϵ�ˣ���˾��ϵGoogle��˾ʱҪ��ϵ���ˣ���Щ�˶���Google��˾��Ա����

### 7-1-2. ��дʵ����
`Customer`
```java
/**
 * @author qinghua
 * @date 2018/9/21 10:42
 */
@Entity //����ʵ����
@Table(name = "cst_customer") //ʵ����ͱ��ӳ���ϵ
public class Customer {

    /**
     * �������ɲ���
     * IDENTITY : ��Ҫ���ݿ�֧���Զ����� (MySQL,SqlServer)
     * SEQUENCE : ��Ҫ���ݿ�֧������ (Oracle)
     * TABLE : ��JPAά��һ�Ŷ�����������
     * AUTO : �������ݿ������Զ�ѡ�����ɲ���
     */
    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    @Column(name = "cust_id")
    private Long custId; //�ͻ���ţ�������
    @Column(name = "cust_name")
    private String custName; //�ͻ����ƣ���˾���ƣ�
    @Column(name = "cust_source")
    private String custSource; //�ͻ���Ϣ��Դ
    @Column(name = "cust_industry")
    private String custIndustry; //�ͻ�������ҵ
    @Column(name = "cust_level")
    private String custLevel; //�ͻ�����
    @Column(name = "cust_address")
    private String custAddress; //�ͻ���ϵ��ַ
    @Column(name = "cust_phone")
    private String custPhone; //�ͻ���ϵ�绰

    /**
     * OneToMay:
     * targetEntity: �Է����ֽ������
     * JoinColumn:
     * name: ����ֶ���
     * referencedColumnName: �����Ӧ�������ֶ���
     */
    @OneToMany(targetEntity = LinkMan.class)
    @JoinColumn(name = "lkm_cust_id", referencedColumnName = "cust_id")
    private Set<LinkMan> linkMans = new HashSet<>();//��ϵ�˼���

    //getter & setter & toString
}
```
<br>
`LinkMan` 
```java
/**
 * @author qinghua
 * @date 2018/9/22 9:47
 */
@Entity
@Table(name = "cst_linkman")
public class LinkMan {

    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    @Column(name = "lkm_id")
    private Long lkmId; //��ϵ�˱��
    @Column(name = "lkm_name")
    private String lkmName; //��ϵ������
    @Column(name = "lkm_gender")
    private String lkmGender; //��ϵ���Ա�
    @Column(name = "lkm_phone")
    private String lkmPhone; //��ϵ�˰칫�绰
    @Column(name = "lkm_mobile")
    private String lkmMobile; //��ϵ���ֻ�
    @Column(name = "lkm_email")
    private String lkmEmail; //��ϵ������
    @Column(name = "lkm_position")
    private String lkmPosition; //��ϵ��ְλ
    @Column(name = "lkm_memo")
    private String lkmMemo; //��ϵ�˱�ע

    /**
     * OneToMay:
     * targetEntity: �Է����ֽ������
     * JoinColumn:
     * name: ����ֶ���
     * referencedColumnName: �����Ӧ�������ֶ���
     */
    @ManyToOne(targetEntity = Customer.class)
    @JoinColumn(name = "lkm_cust_id", referencedColumnName = "cust_id")
    private Customer customer; //��ϵ��������˾

    //getter & setter & toString
}
```

### 7-1-3. �־ò�ӿ�
`CustomerRepository`
```java
/**
 * @author qinghua
 * @date 2018/9/21 10:46
 */
public interface CustomerRepository extends JpaRepository<Customer, Long> {

}
```
<br>
`LinkManRepository`
```java
/**
 * @author qinghua
 * @date 2018/9/22 9:54
 */
public interface LinkManRepository extends JpaRepository<LinkMan, Long> {

}
```

### 7-1-4. �������
��д��������ɿͻ�����ϵ�˵ı������
```java
/**
 * @author qinghua
 * @date 2018/9/22 10:19
 */
@RunWith(SpringJUnit4ClassRunner.class)
@ContextConfiguration(locations = "classpath:applicationContext.xml")
public class OneToManyTest {

    @Autowired
    private CustomerRepository customerRepository;

    @Autowired
    private LinkManRepository linkManRepository;

    /**
     * ���Ա������
     */
    @Test
    @Commit
    public void testSave() {
        //�����ͻ�
        Customer customer = new Customer();
        customer.setCustName("Google");
        customer.setCustIndustry("������");

        //������ϵ��
        LinkMan linkMan = new LinkMan();
        linkMan.setLkmName("�������");
        linkMan.setLkmPhone("13800138000");

        //������ϵ
        customer.getLinkMans().add(linkMan);

        //������ϵ�ˣ�û�����ü�������ʱ����ϵ����Ҫ�ȱ��浽���ݿ⣩
        linkManRepository.save(linkMan);
        //����ͻ�
        customerRepository.save(customer);
    }
}
```

### 7-1-5. �������ά��
���ڣ��ͻ�����ϵ��ʵ�����ж������������ϵ��������ʾ��
`Customer`
```java
@OneToMany(targetEntity = LinkMan.class)
@JoinColumn(name = "lkm_cust_id", referencedColumnName = "cust_id")
private Set<LinkMan> linkMans = new HashSet<>();//��ϵ�˼���
```
<br>
`LinkMan`
```java
@ManyToOne(targetEntity = Customer.class)
@JoinColumn(name = "lkm_cust_id", referencedColumnName = "cust_id")
private Customer customer; //��ϵ��������˾
```
������ʵ���඼���������ϵ��ʱ�򣬱����κ�һ��ʵ����Ķ������ݿ��У�JPA ����ȥά��������������ݿ��е������ϵ��������ı���ʾ���У����Ƿֱ𱣴�������ʵ��Ķ��������ϵ���ᱻά�����Σ���ϵ���ڲ��뵽���ݿ�ʱ����Ѿ�ȷ�������ǿͻ�ʵ�廹Ҫ��ά��һ�Σ���ʱ��෢��һ�� update ��䣬������ʾ��


Ҫ����������Ҳ�ܼ򵥣�����û�б�Ҫ������ʵ�嶼ȥά�������һ������ֶ����ĸ�ʵ�����У�����˭��ά����Ҳ����˵���һ����ά����������ڣ������ÿͻ����������ά��Ȩ�����£�
`Customer`
```java
@Entity
@Table(name = "cst_customer")
public class Customer {

    //��...

    /**
     * OneToMay:
     * mappedBy: ��ʾ��ǰʵ�����ά���������Ĺ�ϵ�����ڶԷ���customer������
     */
    @OneToMany(mappedBy = "customer")
    private Set<LinkMan> linkMans = new HashSet<>();//��ϵ�˼���

    //��...

}
```
<br>
���ͻ����������ά��ȫ֮�󣬱���ͻ�ʱ�Ͳ���������ά����ֻ���ڱ�����ϵ��ʱ�Ż�ά�������������Ҫע��һ�����⣬Ҫ������ϵ�������Ľ������ά���������Ҫ����ϵ��֪�����������Ŀͻ���˭����ܼ򵥣�ֻ��Ҫ����ϵ�˶����еĿͻ����Խ��и�ֵ�ͺ��ˣ����⣬�ڱ�����ϵ��֮ǰ����Ҫ��֤�ͻ��Ѿ������档
�����ǿͻ��������ά��Ȩ֮���ʾ������
```java
/**
 * @author qinghua
 * @date 2018/9/22 10:19
 */
@RunWith(SpringJUnit4ClassRunner.class)
@ContextConfiguration(locations = "classpath:applicationContext.xml")
public class OneToManyTest {

    @Autowired
    private CustomerRepository customerRepository;

    @Autowired
    private LinkManRepository linkManRepository;

    /**
     * ���Ա������
     */
    @Test
    @Commit
    public void testSave() {
        //�����ͻ�
        Customer customer = new Customer();
        customer.setCustName("Google");
        customer.setCustIndustry("������");

        //������ϵ��
        LinkMan linkMan = new LinkMan();
        linkMan.setLkmName("�������");
        linkMan.setLkmPhone("13800138000");

        //������ϵ������Ҫ����ϵ��֪���ͻ���˭����Ϊ�������ϵ����ά����
        linkMan.setCustomer(customer);

        //����ͻ�����û�����ü�������ʱ���ͻ���Ҫ�ȱ��棩
        customerRepository.save(customer);

        //������ϵ��
        linkManRepository.save(linkMan);

    }
}
```

### 7-1-6. ��������
�������õ�ȡֵ
| CascadeType | ˵�� |
| --- |
| CascadeType.ALL | ���в��������� |
| CascadeType.PERSIST | �������� |
| CascadeType.MERGE | �������� |
| CascadeType.REMOVE | ����ɾ�� |
<br>
�����������ĸ�ʵ�����У�
�ȶ�λ`Ҫ����������`�����籣��ͻ���ͬʱ����������ͻ����е���ϵ�ˣ���ô�������������`�ͻ�`�����������ڿͻ�ʵ���༴�ɡ�
<br>
- **��������**
���󣺱���ͻ���ͬʱ����������ͻ���������ϵ��
`Customer` �ļ������ã�
    ```java
    @Entity
    @Table(name = "cst_customer")
    public class Customer {
        
        //��...
        
        /**
         * OneToMay:
         *      cascade = CascadeType.PERSIST ����������
         */
        @OneToMany(cascade = CascadeType.PERSIST)
        @JoinColumn(name = "lkm_cust_id", referencedColumnName = "cust_id")
        private Set<LinkMan> linkMans = new HashSet<>();//��ϵ�˼���
        
        //��...
    }
    ```
<br>
����ʾ�����룺
    ```java
    /**
     * ��������
     */
    @Test
    @Commit
    public void testCascadePersist() {
        //�����ͻ�
        Customer customer = new Customer();
        customer.setCustName("Google");
        customer.setCustIndustry("������");
    
        //������ϵ��
        LinkMan linkMan = new LinkMan();
        linkMan.setLkmName("�������");
        linkMan.setLkmPhone("13800138000");
    
        //��ӹ�ϵ
        customer.getLinkMans().add(linkMan);
    
        //���棨��ʱ�ἶ��������ϵ�ˣ�
        //ע�⣺��ʱ����������ǿͻ������Կͻ����ܷ������ά��
        customerRepository.save(customer);
    }
    ```
<br>
- **����ɾ��**
����ɾ���ͻ���ͬʱɾ���ͻ���������ϵ��
`Customer` �ļ������ã�
    ```java
    @Entity
    @Table(name = "cst_customer")
    public class Customer {
        
        //��...
        
        /**
         * OneToMay:
         *      cascade = CascadeType.REMOVE������ɾ��
         */
        @OneToMany(cascade = CascadeType.REMOVE)
        @JoinColumn(name = "lkm_cust_id", referencedColumnName = "cust_id")
        private Set<LinkMan> linkMans = new HashSet<>();//��ϵ�˼���
        
        //��...
    }
    ```
<br>
����ʾ�����룺
    ```java
    /**
     * ��������
     */
    @Test
    @Commit
    public void testCascadeRemove() {
        //��ѯ�ͻ�
        Customer customer = customerRepository.findById(1L).get();
    
        //ɾ���ͻ�����ʱ�ἶ��ɾ���ÿͻ���������ϵ�ˣ�
        customerRepository.delete(customer);
    }
    ```

## 7-2. ��Զ�
### 7-2-1. ��ȷ���ϵ
- **�û���**
����������...
- **��ɫ��**
ϵͳ����Ա����ͨ�û�...
- **�û�_��ɫ�м��**
�м�������������û��ͽ�ɫ֮��Ķ�Զ�Ĺ�ϵ��

### 7-2-2. ��дʵ����
`User`
```java
/**
 * @author qinghua
 * @date 2018/9/22 15:17
 */
@Entity
@Table(name = "sys_user")
public class User {

    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    @Column(name = "user_id")
    private Long userId;
    @Column(name = "username")
    private String username;
    @Column(name = "password")
    private String password;

    /**
     * ��ǰ�û�ӵ�е����н�ɫ
     *
     * ManyToMany
     * targetEntity: �Է����ֽ������
     *
     * JoinTable
     *      name: �м�������
     *      joinColumns
     *          ��ǰ�������м������
     *     inverseJoinColumns
     *          �Է��������м������
     */
    @ManyToMany(targetEntity = Role.class)
    @JoinTable(name = "sys_user_role",
            joinColumns = {@JoinColumn(name = "user_id", referencedColumnName = "user_id")},
            inverseJoinColumns = {@JoinColumn(name = "role_id", referencedColumnName = "role_id")}
    )
    private Set<Role> roles = new HashSet<>();
    
    //getter & setter & toString
}
```
<br>
`Role`
```java
/**
 * @author qinghua
 * @date 2018/9/22 15:18
 */
@Entity
@Table(name = "sys_role")
public class Role {

    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    @Column(name = "role_id")
    private Long roleId; //��ɫid
    @Column(name = "role_name")
    private String roleName;//��ɫ����

    /**
     * ӵ�е�ǰ��ɫ���û�
     *
     * ManyToMany
     *      targetEntity: �Է����ֽ������
     *
     * JoinTable
     *      name: �м�������
     *      joinColumns
     *          ��ǰ�������м������
     *      inverseJoinColumns
     *          �Է��������м������
     */
    @ManyToMany(targetEntity = User.class)
    @JoinTable(name = "sys_user_role",
            joinColumns = {@JoinColumn(name = "role_id", referencedColumnName = "role_id")},
            inverseJoinColumns = {@JoinColumn(name = "user_id", referencedColumnName = "user_id")}
    )
    private Set<User> users = new HashSet<>();
    
    //getter & setter & toString
}
```

### 7-2-3. �־ò�ӿ�
`UserRepository`
```java
/**
 * @author qinghua
 * @date 2018/9/22 15:29
 */
public interface UserRepository extends JpaRepository<User, Long> {
    
}
```
<br>
`RoleRepository`
```java
/**
 * @author qinghua
 * @date 2018/9/22 15:29
 */
public interface RoleRepository extends JpaRepository<Role, Long> {

}
```

### 7-2-4 �������
```java
/**
 * @author qinghua
 * @date 2018/9/22 15:56
 */
@RunWith(SpringJUnit4ClassRunner.class)
@ContextConfiguration(locations = "classpath:applicationContext.xml")
public class ManyToManyTest {

    @Autowired
    private UserRepository userRepository;

    @Autowired
    private RoleRepository roleRepository;

    /**
     * ����ʵ��
     */
    @Test
    public void testSave() {
        //�����û�
        User user = new User();
        user.setUsername("jack");
        user.setPassword("123");

        //������ɫ
        Role role = new Role();
        role.setRoleName("admin");

        //������ϵ���û���ά�������ϵ��
        user.getRoles().add(role);

        //���ﲻ����˫�����������ά������������м���в�������������¼������������ͻ
        //role.getUsers().add(user);

        //��û�����ü�������֮ǰ����Ҫ�Ƚ���ɫ���浽���ݿ�
        roleRepository.save(role);
        userRepository.save(user);
    }
}
```

### 7-2-5. �������ά��
����ķ�����һ�Զ��������һ���ģ���һ�Զ��ϵ�У����Ǿ�����һ��һ���������ά�����ɶ��һ����ά�����ڶ�Զ��ϵ��˭�������ά��ȡ����˭�Ǳ����ģ�����ǰ�����Ӳ��������ǽ���ɫ��ӵ��û��Ľ�ɫ�б��У���ʱ����ɫ���Ǳ����ģ�˭�Ǳ����ģ�˭�ͷ��������ά��Ȩ��
`Role`
```java
@Entity
@Table(name = "sys_role")
public class Role {

    //��...

    /**
     * ӵ�е�ǰ��ɫ���û�
     *
     * ManyToMany
     * mappedBy: ��ǰʵ��������ά��������Ĺ�ϵ�����ڶԷ��� roles ������
     *
     */
    @ManyToMany(mappedBy = "roles")
    private Set<User> users = new HashSet<>();

    //��...
}
```

### 7-2-6. ��������
�������������ú�һ�Զ������Ҳ��һ���ģ�����������д���ĸ�ʵ�������أ���ȻҪ�ȶ�λ���������壬���磺�����û���ͬʱ������û����еĽ�ɫ����ô��������������û�������������д���û���ʵ�����С�
`User`
```java
@Entity
@Table(name = "sys_user")
public class User {

    //��...

    /**
     * ��ǰ�û�ӵ�е����н�ɫ
     *
     * ManyToMany
     * cascade: ��������������
     */
    @ManyToMany(targetEntity = Role.class, cascade = CascadeType.ALL)
    @JoinTable(name = "sys_user_role",
            joinColumns = {@JoinColumn(name = "user_id", referencedColumnName = "user_id")},
            inverseJoinColumns = {@JoinColumn(name = "role_id", referencedColumnName = "role_id")}
    )
    private Set<Role> roles = new HashSet<>();
    
    //��...
}
```

# 8. ���󵼺���ѯ
## 8-1. ���󵼺���ѯ���ӳټ���
���󵼺���ѯ��ͨ��������÷�������ѯ���������һ�ֲ�ѯ��ʽ������ͨ���ͻ���ѯ�ͻ�����ϵ��
```java
/**
 * @author qinghua
 * @date 2018/9/22 17:12
 */
@RunWith(SpringJUnit4ClassRunner.class)
@ContextConfiguration(locations = "classpath:applicationContext.xml")
public class ObjectQueryTest {

    @Autowired
    private CustomerRepository customerRepository;

    /**
     * ͨ���ͻ���ѯ�ͻ���������ϵ��
     */
    @Test
    @Transactional //no session
    public void testOneFindMany() {
        Customer customer = customerRepository.findById(1L).get();
        Set<LinkMan> linkMans = customer.getLinkMans();//Ĭ���ӳټ���
        System.out.println(linkMans.size());
    }
}
```
<br>
Ĭ������£�`��һ��һ����ѯ���һ��`ʹ�õ���`�ӳټ���`�������Ҫ�������أ��޸�ע�������е� `fetch` ���Լ��ɡ�
���磬����Ķ��󵼺���ѯʾ����ͨ���ͻ�����ѯ��ϵ�ˣ�����ϣ����ѯ����ϵ��ʱ���������س����ģ������Ҫ�ڿͻ�����ϵ�������Ͻ������õ��޸�
`Customer`
```java
@Entity
@Table(name = "cst_customer")
public class Customer {

    //��...

    /**
     * OneToMay
     * fetch ���ز���
     * FetchType.EAGER: ��������
     */
    @OneToMany(cascade = CascadeType.ALL, fetch = FetchType.EAGER)
    @JoinColumn(name = "lkm_cust_id", referencedColumnName = "cust_id")
    private Set<LinkMan> linkMans = new HashSet<>();//��ϵ�˼���

    //��...
}
```

## 8-2. �Ӷ�Ų�ѯһ��
ע�⣬�Ӷ��һ����ѯһ��һ��Ĭ�ϲ��õ����������أ���Ϊ��ѯ������ֻ��һ�������ӳټ��ص����岻�������Ҫ�ӳټ��أ�Ҳ����ͨ�� `fetch` ���ø��ļ��ز��ԡ�
```
@RunWith(SpringJUnit4ClassRunner.class)
@ContextConfiguration(locations = "classpath:applicationContext.xml")
public class ObjectQueryTest {

    @Autowired
    private CustomerRepository customerRepository;

    @Autowired
    private LinkManRepository linkManRepository;

    /**
     * ͨ����ϵ�˲�ѯ�ͻ�
     */
    @Test
    public void testManyFindOne() {
        LinkMan linkMan = linkManRepository.findById(1L).get();
        Customer customer = linkMan.getCustomer();//Ĭ����������
        System.out.println(customer);
    }

}
```
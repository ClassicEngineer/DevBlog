---
title: "Spring Annotations"
date: 2023-07-06T09:26:06+03:00
image: "spring_meme.jpg"
draft: false
# tags:
#   - tagA
#   - tagB
---

Спринг работает... работает автомагически.

Большая часть этой авто-магии настраивается аннотациями.
Поэтому мне захотелось собрать список аннотаций которые являются основными и записать к ним краткий, но важный комментарий
Некоторые остануться без комментария ибо они лежат в core и уже очевидно что делают из своего названия.

### Core
1. @Autowired
2. @Bean
3. @Component
4. @Service
5. @Repository
6. @Configuration
7. @Controller
8. @ActiveProfiles - указывает активные профили
9. @Async - метод будет выполняться асинхронно
10. @ComponentScan - сканирование на поиск бинов
11. @Lazy - ленивая инициализация бина
12. @Job - обьявить джобу
13. @Singleton - антипаттерн))
14. @PostConstruct - функция вызовется после конструктора (см15. @PreAuthorize - auth аспекты
16. @PreDestroy - функция вызовется в конце жизненной цикла бина17. @Primary - выбрать основной бин
18. @Profile - указать профиль
19. @Qualifier - выбрать нужный бин для иньекции
20. @Resource - обозначить ресурс
21. @SpringBootApplication
22. @Scheduled - джоба по cron-расписанию

### Configuration
1. @Import - Для импорта конфигураций одна в другую
2. @ContextConfiguration
3. @SpringJUnitConfig

### Enable

1. @EnableAsync
2. @EnableBatchProcessing
3. @EnableJms
4. @EnableJpaRepositories
5. @EnableScheduling
6. @EnableWebMvc
7. @ЕnаblеWebSocketMessageBroker

### Tests

1. @AfterAll
2. @AfterEach
3. @AssertFalse
4. @AssertTrue
5. @BeforeAll
6. @BeforeEach
7. @ExtendWith
8. @TestExecutionListeners
9. @Test


### Rest

1. @Param
2. @PathVariable
3. @RequestMapping
4. @RequestMapping
5. @RestController

### Data
1. @Column
2. @Entity
3. @Id
4. @JoinColumn
5. @JoinTable
6. @SqlGroup
7. @Sql
8. @ManyToMany
9. @ManyToOne
10. @OneToMany
11. @Query
12. @Repository
13. @PersistenceContext
14. @Таblе

### Transaction
1. @Transactional
2. @AfterTransaction
3. @BeforeTransaction
4. @Rollback
5. @JmsListener - Листенер Java Message System, может слушать например ActiveMq/RabbitMq сообщения


Неизвестные мне:

1. @AdviceRequired
2. @AliasFor
3. @Audited
4. @Basic
5. @ComponentScanning
6. @DataSets
7. @DisplayName
8. @EntityListeners
9. @GeneratedValue
10. @ImportResource
11. @ManagedResource
12. @MappedSuperclass
13. @Named
14. @NotAudited
15. @RunWith
16. @StaticMetamodel
17. @StepScope
18. @Temporal
19. @Transient
20. @Valid
21. @Value
22. @Version

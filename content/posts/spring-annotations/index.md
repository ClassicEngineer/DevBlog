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
16. @Async - метод будет выполняться асинхронно
26. @ComponentScan - сканирование на поиск бинов
51. @Lazy - ленивая инициализация бина
52. @Job - обьявить джобу
79. @Singleton
63. @PostConstruct
64. @PreAuthorize
65. @PreDestroy
66. @Primary
67. @Profile
68. @Qualifier
73. @Resource
80. @SpringBootApplication
77. @Scheduled - джоба по cron-расписанию

### Configuration
46. @Import - Для импорта конфигураций одна в другую
29. @ContextConfiguration
81. @SpringJUnitConfig

### Enable

33. @EnableAsync
34. @EnableBatchProcessing
35. @EnableJms
36. @EnableJpaRepositories
37. @EnableScheduling
38. @EnableWebMvc
39. @ЕnаblеWebSocketMessageBroker

### Tests

10. @AfterAll
11. @AfterEach
14. @AssertFalse
15. @AssertTrue
21. @BeforeAll
22. @BeforeEach
42. @ExtendWith
88. @TestExecutionListeners
89. @Test


### Rest

60. @Param
61. @PathVariable
71. @RequestMapping
72. @RequestMapping
74. @RestController

### Data
24. @Column
41. @Entity
44. @Id
49. @JoinColumn
50. @JoinTable
82. @SqlGroup
83. @Sql
54. @ManyToMany
55. @ManyToOne
59. @OneToMany
69. @Query
70. @Repository
62. @PersistenceContext
86. @Таblе

### Transaction
90. @Transactional
12. @AfterTransaction
23. @BeforeTransaction
75. @Rollback

48. @JmsListener - Листенер Java Message System, может слушать например ActiveMq/RabbitMq сообщения

Неизвестные мне:

9. @AdviceRequired
13. @AliasFor
17. @Audited
19. @Basic
25. @ComponentScanning
31. @DataSets
32. @DisplayName
40. @EntityListeners
43. @GeneratedValue
45. @ImportResource
53. @ManagedResource
56. @MappedSuperclass
57. @Named
58. @NotAudited
76. @RunWith
84. @StaticMetamodel
85. @StepScope
87. @Temporal
91. @Transient
92. @Valid
93. @Value
94. @Version

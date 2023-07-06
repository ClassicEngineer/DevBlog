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

### Configuration
46. @Import - Для импорта конфигураций одна в другую
29. @ContextConfiguration

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




### Data
24. @Column
41. @Entity
44. @Id
49. @JoinColumn
50. @JoinTable
82. @SqlGroup
83. @Sql

### Transaction
90. @Transactional
12. @AfterTransaction


9. @AdviceRequired


13. @AliasFor
17. @Audited
19. @Basic

23. @BeforeTransaction

25. @ComponentScanning



31. @DataSets
32. @DisplayName


40. @EntityListeners


43. @GeneratedValue

45. @ImportResource


48. @JmsListener


53. @ManagedResource
54. @ManyToMany
55. @ManyToOne
56. @MappedSuperclass
57. @Named
58. @NotAudited
59. @OneToMany
60. @Param
61. @PathVariable
62. @PersistenceContext
63. @PostConstruct
64. @PreAuthorize
65. @PreDestroy
66. @Primary
67. @Profile
68. @Qualifier
69. @Query
70. @Repository
71. @RequestMapping
72. @RequestMapping
73. @Resource
74. @RestController
75. @Rollback
76. @RunWith
77. @Scheduled
78. @Service

80. @SpringBootApplication
81. @SpringJUnitConfig

84. @StaticMetamodel
85. @StepScope
86. @Таblе
87. @Temporal
88. @TestExecutionListeners
89. @Test

91. @Transient
92. @Valid
93. @Value
94. @Version

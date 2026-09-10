/* ============================================================
   EngLevel — учебник + тренажёр английского языка (B1-B2)
   ============================================================ */

/* ---------- Утилита: разбить пример на слова с переводом ----------
   sentence задаётся как массив пар [англ.слово_или_знак, перевод]
   Если перевод пустой '' — слово рендерится без подсказки (напр. знаки препинания) */
function ex(pairs){ return pairs; }

/* ==================== ГРАММАТИКА (ТЕОРИЯ) ==================== */
const GRAMMAR = [
{
  id:'parts-of-speech',
  title:'Части речи (Parts of Speech)',
  level:'B1',
  text:`В английском языке, как и в русском, есть основные части речи: существительное (noun), глагол (verb), прилагательное (adjective), наречие (adverb), местоимение (pronoun), предлог (preposition), союз (conjunction) и артикль (article). Понимание частей речи помогает правильно строить предложения и понимать порядок слов.`,
  formula:'Подлежащее (Subject) + Сказуемое (Verb) + Дополнение (Object)',
  examples:[
    ex([['She','она'],['quickly','быстро'],['reads','читает'],['an','—'],['interesting','интересную'],['book','книгу'],['.','']]),
    ex([['My','мой'],['brother','брат'],['works','работает'],['in','в'],['a','—'],['big','большой'],['company','компании'],['.','']])
  ]
},
{
  id:'articles',
  title:'Артикли a / an / the',
  level:'B1',
  text:`Артикль "a/an" ставится перед исчисляемыми существительными в единственном числе, когда предмет упоминается впервые или неважно, какой именно. "The" используется, когда предмет уже известен собеседнику или единственный в своём роде. Перед гласным звуком используется "an".`,
  formula:'a/an + существительное (в первый раз) · the + существительное (уже известно)',
  examples:[
    ex([['I','я'],['saw','увидел'],['a','—'],['dog','собаку'],['.','']]),
    ex([['The','—'],['dog','собака'],['was','была'],['very','очень'],['friendly','дружелюбной'],['.','']])
  ]
},
{
  id:'present-simple',
  title:'Present Simple',
  level:'B1',
  text:`Present Simple используется для регулярных действий, привычек, фактов и расписаний. Глагол в 3-м лице единственного числа получает окончание -s/-es.`,
  formula:'I/You/We/They + V(base) · He/She/It + V(-s/es) · вопрос: Do/Does + подлежащее + V?',
  examples:[
    ex([['She','она'],['works','работает'],['every','каждый'],['day','день'],['.','']]),
    ex([['Do','—'],['you','ты'],['like','любишь'],['coffee','кофе'],['?','']])
  ]
},
{
  id:'present-continuous',
  title:'Present Continuous',
  level:'B1',
  text:`Используется для действий, происходящих прямо сейчас, или для временных ситуаций, а также для запланированных действий в ближайшем будущем.`,
  formula:'подлежащее + am/is/are + V-ing',
  examples:[
    ex([['I','я'],['am','—'],['writing','пишу'],['an','—'],['email','письмо'],['now','сейчас'],['.','']]),
    ex([['They','они'],['are','—'],['meeting','встречаются'],['tomorrow','завтра'],['.','']])
  ]
},
{
  id:'present-perfect',
  title:'Present Perfect',
  level:'B2',
  text:`Используется для действий, которые произошли в прошлом, но связаны с настоящим (результат важен сейчас), либо для опыта без указания точного времени.`,
  formula:'подлежащее + have/has + V3 (Past Participle)',
  examples:[
    ex([['I','я'],['have','—'],['finished','закончил'],['my','мою'],['homework','домашнюю работу'],['.','']]),
    ex([['She','она'],['has','—'],['never','никогда'],['been','не была'],['to','в'],['Paris','Париже'],['.','']])
  ]
},
{
  id:'present-perfect-continuous',
  title:'Present Perfect Continuous',
  level:'B2',
  text:`Подчёркивает длительность действия, которое началось в прошлом и либо продолжается сейчас, либо только что закончилось, но его результат виден.`,
  formula:'подлежащее + have/has + been + V-ing',
  examples:[
    ex([['I','я'],['have','—'],['been','—'],['studying','учусь'],['English','английскому'],['for','уже'],['two','два'],['years','года'],['.','']])
  ]
},
{
  id:'past-simple',
  title:'Past Simple',
  level:'B1',
  text:`Используется для завершённых действий в прошлом с указанием (или подразумеванием) конкретного времени.`,
  formula:'подлежащее + V2 (Past) · вопрос: Did + подлежащее + V(base)?',
  examples:[
    ex([['We','мы'],['visited','посетили'],['London','Лондон'],['last','в прошлом'],['year','году'],['.','']]),
    ex([['Did','—'],['you','ты'],['call','звонил'],['her','ей'],['yesterday','вчера'],['?','']])
  ]
},
{
  id:'past-continuous',
  title:'Past Continuous',
  level:'B1',
  text:`Описывает действие, которое происходило в определённый момент в прошлом, часто в фоне другого события.`,
  formula:'подлежащее + was/were + V-ing',
  examples:[
    ex([['I','я'],['was','—'],['cooking','готовил'],['when','когда'],['he','он'],['called','позвонил'],['.','']])
  ]
},
{
  id:'past-perfect',
  title:'Past Perfect',
  level:'B2',
  text:`Используется для действия, которое произошло раньше другого действия в прошлом ("прошлое до прошлого").`,
  formula:'подлежащее + had + V3',
  examples:[
    ex([['She','она'],['had','—'],['already','уже'],['left','ушла'],['when','когда'],['I','я'],['arrived','приехал'],['.','']])
  ]
},
{
  id:'future-simple',
  title:'Future Simple (will)',
  level:'B1',
  text:`Используется для решений, принятых в момент речи, обещаний, предсказаний.`,
  formula:'подлежащее + will + V(base)',
  examples:[
    ex([['I','я'],['will','—'],['help','помогу'],['you','тебе'],['tomorrow','завтра'],['.','']])
  ]
},
{
  id:'going-to',
  title:'be going to',
  level:'B1',
  text:`Используется для заранее спланированных намерений и для предсказаний на основе явных признаков в настоящем.`,
  formula:'подлежащее + am/is/are + going to + V(base)',
  examples:[
    ex([['We','мы'],['are','—'],['going','—'],['to','—'],['travel','путешествовать'],['next','в следующем'],['month','месяце'],['.','']])
  ]
},
{
  id:'conditional1',
  title:'First Conditional (реальное будущее)',
  level:'B2',
  text:`Описывает реальные, возможные ситуации в будущем и их вероятные последствия.`,
  formula:'If + Present Simple, ... will + V(base)',
  examples:[
    ex([['If','если'],['it','это'],['rains','дождь'],[',',''],['I','я'],['will','—'],['stay','останусь'],['home','дома'],['.','']])
  ]
},
{
  id:'conditional2',
  title:'Second Conditional (нереальное настоящее/будущее)',
  level:'B2',
  text:`Описывает гипотетические, маловероятные или невозможные ситуации в настоящем или будущем.`,
  formula:'If + Past Simple, ... would + V(base)',
  examples:[
    ex([['If','если бы'],['I','я'],['had','имел'],['more','больше'],['time','времени'],[',',''],['I','я'],['would','—'],['travel','путешествовал бы'],['more','больше'],['.','']])
  ]
},
{
  id:'conditional3',
  title:'Third Conditional (нереальное прошлое)',
  level:'B2',
  text:`Описывает гипотетические ситуации в прошлом, которые не произошли, и их воображаемые последствия.`,
  formula:'If + Past Perfect, ... would have + V3',
  examples:[
    ex([['If','если бы'],['I','я'],['had','имел'],['known','знал'],[',',''],['I','я'],['would','—'],['have','—'],['helped','помог бы'],['you','тебе'],['.','']])
  ]
},
{
  id:'passive',
  title:'Passive Voice (страдательный залог)',
  level:'B2',
  text:`Используется, когда важнее само действие или объект, а не тот, кто его совершил.`,
  formula:'подлежащее + to be + V3 (+ by ...)',
  examples:[
    ex([['The','—'],['letter','письмо'],['was','было'],['written','написано'],['by','—'],['Anna','Анной'],['.','']])
  ]
},
{
  id:'modals',
  title:'Модальные глаголы (Modal Verbs)',
  level:'B1',
  text:`Can/could — возможность и умение, must/have to — необходимость, should — совет, may/might — вероятность.`,
  formula:'подлежащее + модальный глагол + V(base)',
  examples:[
    ex([['You','ты'],['should','—'],['drink','пить'],['more','больше'],['water','воды'],['.','']]),
    ex([['She','она'],['can','—'],['speak','говорить'],['three','на трёх'],['languages','языках'],['.','']])
  ]
},
{
  id:'reported-speech',
  title:'Косвенная речь (Reported Speech)',
  level:'B2',
  text:`При передаче чужих слов время глагола обычно "сдвигается назад" (Present → Past, Past → Past Perfect).`,
  formula:'He said that + подлежащее + V(в прошедшем времени)',
  examples:[
    ex([['He','он'],['said','сказал'],['that','что'],['he','он'],['was','был'],['tired','уставшим'],['.','']])
  ]
},
{
  id:'gerund-infinitive',
  title:'Gerund vs Infinitive',
  level:'B2',
  text:`Некоторые глаголы требуют после себя герундий (V-ing), другие — инфинитив (to + V). Это нужно запоминать по конкретным глаголам (enjoy + V-ing, want + to V).`,
  formula:'enjoy/finish/avoid + V-ing · want/decide/plan + to V',
  examples:[
    ex([['I','я'],['enjoy','люблю'],['reading','читать'],['books','книги'],['.','']]),
    ex([['She','она'],['wants','хочет'],['to','—'],['learn','выучить'],['French','французский'],['.','']])
  ]
}
];

/* ==================== СЛОВАРЬ ==================== */
/* формат: [англ, транскрипция, перевод, уровень] */
const DICTIONARY_RAW = [
['achieve','/əˈtʃiːv/','достигать','B2'],
['advice','/ədˈvaɪs/','совет','B1'],
['afford','/əˈfɔːd/','позволить себе','B1'],
['agree','/əˈɡriː/','соглашаться','B1'],
['amazing','/əˈmeɪzɪŋ/','удивительный','B1'],
['ambition','/æmˈbɪʃn/','амбиция','B2'],
['ancient','/ˈeɪnʃənt/','древний','B2'],
['annoy','/əˈnɔɪ/','раздражать','B1'],
['anxious','/ˈæŋkʃəs/','встревоженный','B2'],
['apologize','/əˈpɒlədʒaɪz/','извиняться','B1'],
['appreciate','/əˈpriːʃieɪt/','ценить','B2'],
['approach','/əˈprəʊtʃ/','подход','B2'],
['argue','/ˈɑːɡjuː/','спорить','B1'],
['available','/əˈveɪləbl/','доступный','B1'],
['average','/ˈævərɪdʒ/','средний','B1'],
['avoid','/əˈvɔɪd/','избегать','B1'],
['aware','/əˈweər/','осведомлённый','B2'],
['behave','/bɪˈheɪv/','вести себя','B1'],
['belief','/bɪˈliːf/','убеждение','B2'],
['benefit','/ˈbenɪfɪt/','польза','B1'],
['border','/ˈbɔːdər/','граница','B1'],
['brave','/breɪv/','смелый','B1'],
['breathe','/briːð/','дышать','B1'],
['brilliant','/ˈbrɪliənt/','блестящий','B1'],
['budget','/ˈbʌdʒɪt/','бюджет','B1'],
['cause','/kɔːz/','причина; вызывать','B1'],
['challenge','/ˈtʃælɪndʒ/','вызов, трудность','B1'],
['chase','/tʃeɪs/','преследовать','B1'],
['cheerful','/ˈtʃɪəfl/','весёлый','B1'],
['clever','/ˈklevər/','умный','B1'],
['collapse','/kəˈlæps/','рушиться','B2'],
['combine','/kəmˈbaɪn/','сочетать','B2'],
['comfort','/ˈkʌmfət/','комфорт','B1'],
['compare','/kəmˈpeər/','сравнивать','B1'],
['complain','/kəmˈpleɪn/','жаловаться','B1'],
['confident','/ˈkɒnfɪdənt/','уверенный','B1'],
['confuse','/kənˈfjuːz/','запутывать','B1'],
['consider','/kənˈsɪdər/','считать, рассматривать','B2'],
['consist','/kənˈsɪst/','состоять','B2'],
['convince','/kənˈvɪns/','убеждать','B2'],
['crucial','/ˈkruːʃl/','решающий, важный','B2'],
['curious','/ˈkjʊəriəs/','любопытный','B1'],
['damage','/ˈdæmɪdʒ/','повреждение','B1'],
['deal','/diːl/','сделка; иметь дело','B1'],
['decade','/ˈdekeɪd/','десятилетие','B1'],
['decision','/dɪˈsɪʒn/','решение','B1'],
['delay','/dɪˈleɪ/','задержка','B1'],
['demand','/dɪˈmɑːnd/','требовать','B2'],
['deny','/dɪˈnaɪ/','отрицать','B2'],
['depend','/dɪˈpend/','зависеть','B1'],
['describe','/dɪˈskraɪb/','описывать','B1'],
['determine','/dɪˈtɜːmɪn/','определять','B2'],
['develop','/dɪˈveləp/','развивать','B1'],
['disappoint','/ˌdɪsəˈpɔɪnt/','разочаровывать','B1'],
['discover','/dɪˈskʌvər/','обнаруживать','B1'],
['doubt','/daʊt/','сомнение','B1'],
['effort','/ˈefət/','усилие','B1'],
['embarrass','/ɪmˈbærəs/','смущать','B2'],
['encourage','/ɪnˈkʌrɪdʒ/','поощрять','B1'],
['environment','/ɪnˈvaɪrənmənt/','окружающая среда','B1'],
['equal','/ˈiːkwəl/','равный','B1'],
['essential','/ɪˈsenʃl/','важный, необходимый','B2'],
['exhausted','/ɪɡˈzɔːstɪd/','измотанный','B2'],
['expect','/ɪkˈspekt/','ожидать','B1'],
['experience','/ɪkˈspɪəriəns/','опыт','B1'],
['explain','/ɪkˈspleɪn/','объяснять','B1'],
['fair','/feər/','справедливый','B1'],
['fascinating','/ˈfæsɪneɪtɪŋ/','увлекательный','B2'],
['fault','/fɔːlt/','вина, ошибка','B1'],
['fear','/fɪər/','страх','B1'],
['flexible','/ˈfleksəbl/','гибкий','B2'],
['focus','/ˈfəʊkəs/','сосредотачиваться','B1'],
['fortunate','/ˈfɔːtʃənət/','удачливый','B2'],
['frustrated','/frʌˈstreɪtɪd/','разочарованный, расстроенный','B2'],
['gain','/ɡeɪn/','получать, приобретать','B1'],
['generous','/ˈdʒenərəs/','щедрый','B1'],
['genuine','/ˈdʒenjuɪn/','настоящий, искренний','B2'],
['goal','/ɡəʊl/','цель','B1'],
['grateful','/ˈɡreɪtfl/','благодарный','B1'],
['guilty','/ˈɡɪlti/','виновный','B1'],
['habit','/ˈhæbɪt/','привычка','B1'],
['handle','/ˈhændl/','справляться','B1'],
['harm','/hɑːm/','вред','B1'],
['honest','/ˈɒnɪst/','честный','B1'],
['hope','/həʊp/','надеяться','B1'],
['identify','/aɪˈdentɪfaɪ/','определять, узнавать','B2'],
['ignore','/ɪɡˈnɔːr/','игнорировать','B1'],
['immediate','/ɪˈmiːdiət/','немедленный','B2'],
['improve','/ɪmˈpruːv/','улучшать','B1'],
['include','/ɪnˈkluːd/','включать','B1'],
['increase','/ɪnˈkriːs/','увеличивать','B1'],
['independent','/ˌɪndɪˈpendənt/','независимый','B1'],
['influence','/ˈɪnfluəns/','влияние','B2'],
['insist','/ɪnˈsɪst/','настаивать','B2'],
['inspire','/ɪnˈspaɪər/','вдохновлять','B2'],
['instead','/ɪnˈsted/','вместо','B1'],
['involve','/ɪnˈvɒlv/','вовлекать','B2'],
['issue','/ˈɪʃuː/','проблема, вопрос','B1'],
['jealous','/ˈdʒeləs/','ревнивый','B1'],
['journey','/ˈdʒɜːni/','путешествие','B1'],
['judge','/dʒʌdʒ/','судить','B1'],
['justify','/ˈdʒʌstɪfaɪ/','оправдывать','B2'],
['knowledge','/ˈnɒlɪdʒ/','знание','B1'],
['lack','/læk/','нехватка','B1'],
['likely','/ˈlaɪkli/','вероятный','B1'],
['maintain','/meɪnˈteɪn/','поддерживать','B2'],
['manage','/ˈmænɪdʒ/','справляться, управлять','B1'],
['mention','/ˈmenʃn/','упоминать','B1'],
['mistake','/mɪˈsteɪk/','ошибка','B1'],
['nervous','/ˈnɜːvəs/','нервный','B1'],
['notice','/ˈnəʊtɪs/','замечать','B1'],
['obvious','/ˈɒbviəs/','очевидный','B1'],
['occur','/əˈkɜːr/','происходить','B2'],
['opportunity','/ˌɒpəˈtjuːnəti/','возможность','B1'],
['opposite','/ˈɒpəzɪt/','противоположный','B1'],
['organize','/ˈɔːɡənaɪz/','организовывать','B1'],
['overcome','/ˌəʊvəˈkʌm/','преодолевать','B2'],
['particular','/pəˈtɪkjələr/','особый, конкретный','B1'],
['patient','/ˈpeɪʃnt/','терпеливый','B1'],
['permanent','/ˈpɜːmənənt/','постоянный','B2'],
['persuade','/pəˈsweɪd/','убеждать','B2'],
['pleasant','/ˈpleznt/','приятный','B1'],
['pressure','/ˈpreʃər/','давление','B1'],
['prevent','/prɪˈvent/','предотвращать','B1'],
['proud','/praʊd/','гордый','B1'],
['purpose','/ˈpɜːpəs/','цель, назначение','B1'],
['reach','/riːtʃ/','достигать','B1'],
['realize','/ˈriːəlaɪz/','осознавать','B1'],
['recognize','/ˈrekəɡnaɪz/','узнавать, признавать','B1'],
['reduce','/rɪˈdjuːs/','сокращать','B1'],
['reject','/rɪˈdʒekt/','отвергать','B2'],
['relationship','/rɪˈleɪʃnʃɪp/','отношения','B1'],
['relevant','/ˈreləvənt/','актуальный, релевантный','B2'],
['reliable','/rɪˈlaɪəbl/','надёжный','B2'],
['relief','/rɪˈliːf/','облегчение','B2'],
['reluctant','/rɪˈlʌktənt/','неохотный','B2'],
['remind','/rɪˈmaɪnd/','напоминать','B1'],
['require','/rɪˈkwaɪər/','требовать','B1'],
['resource','/rɪˈsɔːs/','ресурс','B1'],
['respond','/rɪˈspɒnd/','отвечать, реагировать','B1'],
['responsible','/rɪˈspɒnsəbl/','ответственный','B1'],
['reveal','/rɪˈviːl/','раскрывать','B2'],
['rude','/ruːd/','грубый','B1'],
['satisfied','/ˈsætɪsfaɪd/','довольный','B1'],
['scared','/skeərd/','напуганный','B1'],
['sensible','/ˈsensəbl/','разумный','B2'],
['separate','/ˈsepərət/','отдельный','B1'],
['sharp','/ʃɑːp/','острый, резкий','B1'],
['shy','/ʃaɪ/','застенчивый','B1'],
['similar','/ˈsɪmələr/','похожий','B1'],
['skill','/skɪl/','навык','B1'],
['solve','/sɒlv/','решать','B1'],
['stubborn','/ˈstʌbən/','упрямый','B2'],
['succeed','/səkˈsiːd/','преуспевать','B1'],
['suggest','/səˈdʒest/','предлагать','B1'],
['suitable','/ˈsuːtəbl/','подходящий','B1'],
['support','/səˈpɔːt/','поддерживать','B1'],
['suppose','/səˈpəʊz/','предполагать','B1'],
['surround','/səˈraʊnd/','окружать','B2'],
['suspicious','/səˈspɪʃəs/','подозрительный','B2'],
['tend','/tend/','иметь тенденцию','B2'],
['thorough','/ˈθʌrə/','тщательный','B2'],
['threat','/θret/','угроза','B2'],
['tough','/tʌf/','трудный, жёсткий','B1'],
['unique','/juˈniːk/','уникальный','B1'],
['upset','/ʌpˈset/','расстроенный','B1'],
['urgent','/ˈɜːdʒənt/','срочный','B1'],
['value','/ˈvæljuː/','ценность','B1'],
['various','/ˈveəriəs/','различные','B1'],
['wonder','/ˈwʌndər/','интересоваться, удивляться','B1'],
['worth','/wɜːθ/','стоящий','B1']
];

const DICTIONARY = DICTIONARY_RAW.map(([en,transcr,ru,level])=>({en,transcr,ru,level}));

/* ==================== БАНК ТЕСТОВ (ГРАММАТИКА) ==================== */
const QUIZ_BANK = [
{level:'B1', q:'She ___ to work every day.', options:['go','goes','going','gone'], correct:1, topic:'Present Simple'},
{level:'B1', q:'Right now, I ___ dinner.', options:['cook','cooks','am cooking','cooked'], correct:2, topic:'Present Continuous'},
{level:'B1', q:'We ___ to Italy last summer.', options:['go','went','have gone','goes'], correct:1, topic:'Past Simple'},
{level:'B1', q:'While I ___ TV, the phone rang.', options:['watched','was watching','watch','have watched'], correct:1, topic:'Past Continuous'},
{level:'B1', q:'I promise I ___ help you tomorrow.', options:['will','am','was','did'], correct:0, topic:'Future Simple'},
{level:'B1', q:'Choose the correct article: I saw ___ elephant at the zoo.', options:['a','an','the','-'], correct:1, topic:'Articles'},
{level:'B1', q:'You ___ smoke here, it is forbidden.', options:['can','must not','should','may'], correct:1, topic:'Modal Verbs'},
{level:'B1', q:'They ___ finished their homework yet? (question)', options:['Do','Did','Have','Has'], correct:2, topic:'Present Perfect'},
{level:'B2', q:'I ___ never ___ sushi before yesterday.', options:['have / eaten','had / eaten','has / eaten','was / eating'], correct:1, topic:'Past Perfect'},
{level:'B2', q:'If it rains tomorrow, I ___ stay home.', options:['will','would','had','was'], correct:0, topic:'First Conditional'},
{level:'B2', q:'If I ___ more money, I would travel the world.', options:['have','had','has','will have'], correct:1, topic:'Second Conditional'},
{level:'B2', q:'If she had studied harder, she ___ passed the exam.', options:['would','would have','will have','had'], correct:1, topic:'Third Conditional'},
{level:'B2', q:'The book ___ by millions of people.', options:['reads','has read','has been read','is reading'], correct:2, topic:'Passive Voice'},
{level:'B2', q:'He said that he ___ tired.', options:['is','was','be','being'], correct:1, topic:'Reported Speech'},
{level:'B2', q:'She enjoys ___ books in her free time.', options:['read','to read','reading','reads'], correct:2, topic:'Gerund/Infinitive'},
{level:'B2', q:'I have been ___ English for three years.', options:['study','studied','studying','studies'], correct:2, topic:'Present Perfect Continuous'},
{level:'B1', q:'This is ___ interesting movie I have ever seen.', options:['a','an','the','most'], correct:2, topic:'Articles'},
{level:'B1', q:'We ___ going to visit our grandparents next week.', options:['is','am','are','be'], correct:2, topic:'be going to'},
{level:'B2', q:'You ___ have called me — I was worried!', options:['should','can','must','might'], correct:0, topic:'Modal Verbs'},
{level:'B1', q:'___ you like some tea?', options:['Do','Would','Are','Did'], correct:1, topic:'Polite requests'}
];

/* ==================== СОСТОЯНИЕ ==================== */
let currentLevel = 'all';
let currentPage = 'home';

const app = document.getElementById('app');
const levelSelect = document.getElementById('levelSelect');
const navButtons = document.querySelectorAll('.nav-btn');

levelSelect.addEventListener('change', ()=>{
  currentLevel = levelSelect.value;
  render();
});

navButtons.forEach(btn=>{
  btn.addEventListener('click', ()=>{
    navButtons.forEach(b=>b.classList.remove('active'));
    btn.classList.add('active');
    currentPage = btn.dataset.page;
    render();
  });
});

function filterByLevel(arr){
  if(currentLevel==='all') return arr;
  return arr.filter(item => item.level === currentLevel);
}

/* ==================== РЕНДЕР ПРИМЕРА СО СЛОВАМИ-ПОДСКАЗКАМИ ==================== */
function renderExample(pairs){
  const div = document.createElement('div');
  div.className = 'example';
  pairs.forEach(([en,ru])=>{
    const span = document.createElement('span');
    if(ru){
      span.className = 'word';
      span.innerHTML = en + ' <span class="tr">'+ru+'</span>';
      span.addEventListener('click', ()=> span.classList.toggle('show'));
    } else {
      span.textContent = en + ' ';
      span.style.marginRight = '2px';
    }
    div.appendChild(span);
    div.append(' ');
  });
  return div;
}

/* ==================== ГЛАВНАЯ ==================== */
function renderHome(){
  app.innerHTML = `
    <h1>Добро пожаловать в EngLevel 👋</h1>
    <p class="muted">Учебник + тренажёр английского языка, нацеленный на уровень B1-B2.</p>
    <div class="grid" style="margin-top:20px;">
      <div class="tile" data-go="theory"><h3>📖 Теория</h3><p class="muted">Все основные времена, артикли, пассив, условные предложения и другие темы с примерами.</p></div>
      <div class="tile" data-go="dictionary"><h3>🔤 Словарь</h3><p class="muted">Полезные слова по алфавиту с транскрипцией и переводом.</p></div>
      <div class="tile" data-go="practice"><h3>✏️ Практика</h3><p class="muted">Тесты и упражнения на сопоставление с моментальной проверкой.</p></div>
      <div class="tile" data-go="ai"><h3>🤖 ИИ-помощник</h3><p class="muted">Задай вопрос про грамматику или попроси объяснить слово.</p></div>
    </div>
    <div class="card" style="margin-top:20px;">
      <h2>Как пользоваться</h2>
      <p class="muted">Клик по слову в примерах показывает перевод. Уровень (B1/B2) можно выбрать вверху страницы — теория, словарь и тесты отфильтруются автоматически.</p>
    </div>
  `;
  app.querySelectorAll('.tile').forEach(t=>{
    t.addEventListener('click', ()=>{
      const page = t.dataset.go;
      navButtons.forEach(b=>b.classList.toggle('active', b.dataset.page===page));
      currentPage = page;
      render();
    });
  });
}

/* ==================== ТЕОРИЯ ==================== */
function renderTheoryList(){
  const topics = filterByLevel(GRAMMAR);
  app.innerHTML = `
    <h1>Теория</h1>
    <p class="muted">Выбери тему, чтобы посмотреть правило, формулу и примеры.</p>
    <div class="grid" id="topicGrid"></div>
  `;
  const grid = document.getElementById('topicGrid');
  topics.forEach(t=>{
    const tile = document.createElement('div');
    tile.className = 'tile';
    tile.innerHTML = `<span class="tag ${t.level==='B2'?'b2':''}">${t.level}</span><h3>${t.title}</h3>`;
    tile.addEventListener('click', ()=> renderTheoryDetail(t.id));
    grid.appendChild(tile);
  });
}

function renderTheoryDetail(id){
  const topic = GRAMMAR.find(g=>g.id===id);
  app.innerHTML = '';
  const back = document.createElement('button');
  back.className = 'back-btn';
  back.textContent = '← Назад к темам';
  back.addEventListener('click', renderTheoryList);
  app.appendChild(back);

  const card = document.createElement('div');
  card.className = 'card';
  card.innerHTML = `
    <span class="tag ${topic.level==='B2'?'b2':''}">${topic.level}</span>
    <h2>${topic.title}</h2>
    <p>${topic.text}</p>
    <div class="formula">${topic.formula}</div>
    <h3 style="margin-top:16px;font-size:15px;color:var(--muted);">Примеры (клик по слову — перевод):</h3>
  `;
  topic.examples.forEach(pairs=> card.appendChild(renderExample(pairs)));
  app.appendChild(card);
}

/* ==================== СЛОВАРЬ ==================== */
let dictLetter = 'ALL';
let dictSearch = '';

function renderDictionary(){
  const letters = ['ALL', ...Array.from(new Set(DICTIONARY.map(w=>w.en[0].toUpperCase()))).sort()];
  app.innerHTML = `
    <h1>Словарь</h1>
    <input type="text" class="search-box" id="dictSearch" placeholder="Поиск слова (англ. или рус.)..." value="${dictSearch}">
    <div class="alphabet" id="alphabet"></div>
    <div class="card" id="dictList"></div>
  `;
  const alphaDiv = document.getElementById('alphabet');
  letters.forEach(l=>{
    const b = document.createElement('button');
    b.className = 'letter-btn' + (l===dictLetter ? ' active' : '');
    b.textContent = l==='ALL' ? '☰' : l;
    b.addEventListener('click', ()=>{ dictLetter = l; renderDictionary(); });
    alphaDiv.appendChild(b);
  });

  document.getElementById('dictSearch').addEventListener('input', (e)=>{
    dictSearch = e.target.value.toLowerCase();
    renderDictList();
  });

  renderDictList();
}

function renderDictList(){
  let words = filterByLevel(DICTIONARY);
  if(dictLetter !== 'ALL') words = words.filter(w=> w.en[0].toUpperCase() === dictLetter);
  if(dictSearch) words = words.filter(w=> w.en.toLowerCase().includes(dictSearch) || w.ru.toLowerCase().includes(dictSearch));

  const list = document.getElementById('dictList');
  list.innerHTML = '';
  if(words.length===0){
    list.innerHTML = '<p class="muted">Ничего не найдено.</p>';
    return;
  }
  words.forEach(w=>{
    const row = document.createElement('div');
    row.className = 'dict-item';
    row.innerHTML = `
      <div><span class="en">${w.en}</span><span class="transcr">${w.transcr}</span></div>
      <div style="display:flex;align-items:center;gap:8px;">
        <span class="tr-text hidden">${w.ru}</span>
        <button class="reveal-btn">Показать перевод</button>
      </div>
    `;
    const trSpan = row.querySelector('.tr-text');
    const btn = row.querySelector('.reveal-btn');
    btn.addEventListener('click', ()=>{
      trSpan.classList.toggle('hidden');
      btn.textContent = trSpan.classList.contains('hidden') ? 'Показать перевод' : 'Скрыть';
    });
    list.appendChild(row);
  });
}

/* ==================== ПРАКТИКА ==================== */
function renderPractice(){
  app.innerHTML = `
    <h1>Практика</h1>
    <p class="muted">Выбери тип упражнения:</p>
    <div class="grid">
      <div class="tile" id="goQuiz"><h3>📝 Тест (грамматика)</h3><p class="muted">Выбери правильный вариант ответа.</p></div>
      <div class="tile" id="goMatch"><h3>🔗 Сопоставление слов</h3><p class="muted">Соедини английское слово с переводом.</p></div>
    </div>
  `;
  document.getElementById('goQuiz').addEventListener('click', renderQuiz);
  document.getElementById('goMatch').addEventListener('click', renderMatching);
}

function shuffle(arr){
  const a = [...arr];
  for(let i=a.length-1;i>0;i--){
    const j = Math.floor(Math.random()*(i+1));
    [a[i],a[j]]=[a[j],a[i]];
  }
  return a;
}

/* ---- Тест (multiple choice) ---- */
function renderQuiz(){
  const pool = shuffle(filterByLevel(QUIZ_BANK)).slice(0,8);
  let score = 0;
  let answered = 0;

  app.innerHTML = '';
  const back = document.createElement('button');
  back.className = 'back-btn';
  back.textContent = '← Назад';
  back.addEventListener('click', renderPractice);
  app.appendChild(back);

  const header = document.createElement('div');
  header.className = 'card';
  header.innerHTML = `<h2>Тест по грамматике</h2><p class="muted">Вопросов: ${pool.length}. Нажми на вариант ответа.</p>`;
  app.appendChild(header);

  if(pool.length===0){
    const w = document.createElement('p');
    w.className='muted';
    w.textContent='Для выбранного уровня пока нет вопросов.';
    app.appendChild(w);
    return;
  }

  pool.forEach((q,idx)=>{
    const card = document.createElement('div');
    card.className = 'card q-card';
    card.innerHTML = `<span class="tag ${q.level==='B2'?'b2':''}">${q.level} · ${q.topic}</span><h3>${idx+1}. ${q.q}</h3>`;
    const optWrap = document.createElement('div');
    optWrap.className = 'options';
    q.options.forEach((opt,oi)=>{
      const o = document.createElement('div');
      o.className = 'option';
      o.textContent = opt;
      o.addEventListener('click', ()=>{
        if(o.classList.contains('disabled')) return;
        optWrap.querySelectorAll('.option').forEach(el=>el.classList.add('disabled'));
        if(oi === q.correct){
          o.classList.add('correct');
          score++;
        } else {
          o.classList.add('wrong');
          optWrap.children[q.correct].classList.add('correct');
        }
        answered++;
        if(answered === pool.length) showQuizResult(score, pool.length);
      });
      optWrap.appendChild(o);
    });
    card.appendChild(optWrap);
    app.appendChild(card);
  });

  const resultDiv = document.createElement('div');
  resultDiv.id = 'quizResult';
  app.appendChild(resultDiv);
}

function showQuizResult(score, total){
  const div = document.getElementById('quizResult');
  const pct = Math.round(score/total*100);
  const cls = pct>=70 ? 'good' : 'bad';
  div.innerHTML = `<div class="result-banner ${cls}">Результат: ${score} из ${total} (${pct}%)</div>
    <button class="btn" id="retryQuiz">Пройти ещё раз</button>`;
  document.getElementById('retryQuiz').addEventListener('click', renderQuiz);
}

/* ---- Сопоставление (matching) ---- */
function renderMatching(){
  const words = shuffle(filterByLevel(DICTIONARY)).slice(0,6);

  app.innerHTML = '';
  const back = document.createElement('button');
  back.className = 'back-btn';
  back.textContent = '← Назад';
  back.addEventListener('click', renderPractice);
  app.appendChild(back);

  const header = document.createElement('div');
  header.className = 'card';
  header.innerHTML = `<h2>Сопоставь слово и перевод</h2><p class="muted">Нажми на английское слово, затем на нужный перевод.</p>`;
  app.appendChild(header);

  if(words.length===0){
    const w = document.createElement('p');
    w.className='muted';
    w.textContent='Для выбранного уровня пока нет слов.';
    app.appendChild(w);
    return;
  }

  const card = document.createElement('div');
  card.className = 'card';
  const grid = document.createElement('div');
  grid.className = 'match-grid';
  const leftCol = document.createElement('div');
  leftCol.className = 'match-col';
  const rightCol = document.createElement('div');
  rightCol.className = 'match-col';

  const rightShuffled = shuffle(words);
  let selectedLeft = null;
  let matchedCount = 0;

  words.forEach(w=>{
    const item = document.createElement('div');
    item.className = 'match-item';
    item.textContent = w.en;
    item.dataset.en = w.en;
    item.addEventListener('click', ()=>{
      if(item.classList.contains('matched')) return;
      leftCol.querySelectorAll('.match-item').forEach(el=>el.classList.remove('selected'));
      item.classList.add('selected');
      selectedLeft = item;
    });
    leftCol.appendChild(item);
  });

  rightShuffled.forEach(w=>{
    const item = document.createElement('div');
    item.className = 'match-item';
    item.textContent = w.ru;
    item.dataset.en = w.en;
    item.addEventListener('click', ()=>{
      if(item.classList.contains('matched') || !selectedLeft) return;
      if(item.dataset.en === selectedLeft.dataset.en){
        item.classList.add('matched');
        selectedLeft.classList.add('matched');
        selectedLeft.classList.remove('selected');
        matchedCount++;
        selectedLeft = null;
        if(matchedCount === words.length) showMatchResult();
      } else {
        item.classList.add('wrong-flash');
        selectedLeft.classList.add('wrong-flash');
        setTimeout(()=>{
          item.classList.remove('wrong-flash');
          selectedLeft && selectedLeft.classList.remove('wrong-flash');
        },500);
      }
    });
    rightCol.appendChild(item);
  });

  grid.appendChild(leftCol);
  grid.appendChild(rightCol);
  card.appendChild(grid);
  app.appendChild(card);

  const resultDiv = document.createElement('div');
  resultDiv.id = 'matchResult';
  app.appendChild(resultDiv);

  function showMatchResult(){
    const div = document.getElementById('matchResult');
    div.innerHTML = `<div class="result-banner good">Отлично! Все слова сопоставлены верно 🎉</div>
      <button class="btn" id="retryMatch">Ещё раз с новыми словами</button>`;
    document.getElementById('retryMatch').addEventListener('click', renderMatching);
  }
}

/* ==================== ИИ-ПОМОЩНИК ==================== */
function renderAI(){
  const savedKey = localStorage.getItem('ai_api_key') || '';
  const savedEndpoint = localStorage.getItem('ai_endpoint') || 'https://api.openai.com/v1/chat/completions';

  app.innerHTML = `
    <h1>ИИ-помощник</h1>
    <div class="warn">
      Сайт статический (GitHub Pages), поэтому у него нет своего сервера и своего секретного ИИ-ключа.
      Чтобы ИИ-помощник работал, впиши <b>свой</b> API-ключ (например, от OpenAI) — он хранится только в
      твоём браузере (localStorage) и никуда, кроме выбранного API, не отправляется.
      Если ключа нет — можно пользоваться теорией, словарём и тестами без ИИ.
    </div>
    <div class="card ai-box">
      <label class="muted">Endpoint API (по умолчанию OpenAI chat/completions):</label>
      <input type="text" id="aiEndpoint" value="${savedEndpoint}">
      <label class="muted">Твой API-ключ:</label>
      <input type="password" id="aiKey" value="${savedKey}" placeholder="sk-...">
      <label class="muted">Вопрос (о грамматике, слове, переводе и т.д.):</label>
      <textarea id="aiQuestion" rows="3" placeholder="Например: объясни разницу между Present Perfect и Past Simple с примерами"></textarea>
      <button class="btn" id="aiSend">Спросить</button>
      <div class="ai-log" id="aiLog">Ответ появится здесь...</div>
    </div>
  `;

  document.getElementById('aiSend').addEventListener('click', async ()=>{
    const endpoint = document.getElementById('aiEndpoint').value.trim();
    const key = document.getElementById('aiKey').value.trim();
    const question = document.getElementById('aiQuestion').value.trim();
    const log = document.getElementById('aiLog');

    if(!key){ log.textContent = 'Введи API-ключ, чтобы использовать ИИ-помощника.'; return; }
    if(!question){ log.textContent = 'Напиши вопрос.'; return; }

    localStorage.setItem('ai_api_key', key);
    localStorage.setItem('ai_endpoint', endpoint);

    log.textContent = 'Думаю...';

    try{
      const res = await fetch(endpoint, {
        method:'POST',
        headers:{
          'Content-Type':'application/json',
          'Authorization': 'Bearer ' + key
        },
        body: JSON.stringify({
          model:'gpt-4o-mini',
          messages:[
            {role:'system', content:'Ты — преподаватель английского языка для русскоговорящих учеников уровня B1-B2. Объясняй понятно, кратко, с примерами и переводом на русский.'},
            {role:'user', content:question}
          ]
        })
      });
      if(!res.ok){
        const errText = await res.text();
        log.textContent = 'Ошибка запроса (' + res.status + '). Проверь ключ/эндпоинт.\n' + errText.slice(0,300);
        return;
      }
      const data = await res.json();
      const answer = data.choices?.[0]?.message?.content || JSON.stringify(data);
      log.textContent = answer;
    } catch(err){
      log.textContent = 'Не удалось выполнить запрос. Возможно, сайт с GitHub Pages блокируется политикой CORS этого API, или проблема с сетью.\n' + err.message;
    }
  });
}

/* ==================== ГЛАВНЫЙ РЕНДЕР ==================== */
function render(){
  if(currentPage==='home') renderHome();
  else if(currentPage==='theory') renderTheoryList();
  else if(currentPage==='dictionary') renderDictionary();
  else if(currentPage==='practice') renderPractice();
  else if(currentPage==='ai') renderAI();
}

render();

# Лабораторная работа №1

### Вариант: 385

### Задание:

Электронная библиотека book-online.com.ua: художественная, учебная, деловая литература, справочники - http://book-online.com.ua/

Составить список требований, предъявляемых к разрабатываемому веб-сайту (в соответствии с вариантом). Требования должны делиться на следующие категории:
- Функциональные.
	- Требования пользователей сайта.
	- Требования владельцев сайта.
- Нефункциональные.

Требования необходимо оформить в соответствии с шаблонами RUP (документ SRS - Software Requirements Specification). Для каждого из требований нужно указать его атрибуты (в соответствии с методологией RUP), а также оценить и аргументировать приблизительное количество часов, требующихся на реализацию этого требования.

Для функциональных требований нужно составить UML UseCase-диаграммы, описывающие реализующие их прецеденты использования.

**Отчёт по лабораторной работе должен содержать:**

1. Документ Software Requirements Specification, содержащий список требований к сайту.
2. UseCase-диаграммы прецедентов использования, реализующих функциональные требования.
3. Выводы по работе.

**Вопросы к защите лабораторной работы:**

1. Методологии разработки ПО. Унифицированный процесс.
2. Требования и их категоризация. Атрибуты требований.
3. Язык UML.
4. Прецеденты использования. UseCase-диаграммы - состав, виды связей.
------------


# Лабораторная работа №2

### Вариант: 3300

### Задание:

Сконфигурировать в своём домашнем каталоге репозитории svn и git и загрузить в них начальную ревизию файлов с исходными кодами (в соответствии с выданным вариантом).

Воспроизвести последовательность команд для систем контроля версий svn и git, осуществляющих операции над исходным кодом, приведённые на блок-схеме.

При составлении последовательности команд необходимо учитывать следующие условия:

1. Цвет элементов схемы указывает на пользователя, совершившего действие (красный - первый, синий - второй).
2. Цифры над узлами - номер ревизии. Ревизии создаются последовательно.
3. Необходимо разрешать конфликты между версиями, если они возникают.

**Отчёт по работе должен содержать:**

1. Задание и блок-схему в соответствии с вариантом.
2. Список команд, использованных при создании и конфигурации репозиториев в домашнем каталоге пользователя.
3. Номера ревизий и соответствующие им последовательности команд с комментариями (для svn и git).
4. Выводы по работе.

**Вопросы к защите лабораторной работы:**

1. Системы контроля версий - назначение, примеры решений.
2. Ревизии и ветки.
3. Основные операции над данными в системах контроля версий. Основные команды svn и git.
4. Виды конфликтов и способы их решения.
------------


# Лабораторная работа №3

### Вариант: 55222

### Задание:

Написать сценарий для утилиты Apache Ant, реализующий компиляцию, тестирование и упаковку в jar-архив кода проекта из лабораторной работы №3 по дисциплине "Веб-программирование".

Каждый этап должен быть выделен в отдельный блок сценария; все переменные и константы, используемые в сценарии, должны быть вынесены в отдельный файл параметров; MANIFEST.MF должен содержать информацию о версии и о запускаемом классе.

**Cценарий должен реализовывать следующие цели (targets):**

1. **compile** -- компиляция исходных кодов проекта.
2. **build** -- компиляция исходных кодов проекта и их упаковка в исполняемый jar-архив. Компиляцию исходных кодов реализовать посредством вызова цели compile.
3. **clean** -- удаление скомпилированных классов проекта и всех временных файлов (если они есть).
4. **test** -- запуск junit-тестов проекта. Перед запуском тестов необходимо осуществить сборку проекта (цель build).
5. **xml** - валидация всех xml-файлов в проекте.
6. **team** - осуществляет получение из svn-репозитория 4 предыдущих ревизий, их сборку (по аналогии с основной) и упаковку получившихся jar-файлов в zip-архив. Сборку реализовать посредством вызова цели build.

**Вопросы к защите лабораторной работы:**

1. Тестирование ПО. Цель тестирования, виды тестирования.
2. Модульное тестирование, основные принципы и используемые подходы.
3. Пакет JUnit, основные API.
4. Системы автоматической сборки. Назначение, принципы работы, примеры систем.
5. Утилита make. Make-файлы, цели и правила.
6. Утилита Ant. Сценарии сборки, цели и команды.

------------

# Лабораторная работа №4

### Вариант: 666333

### Задание:

1. Для своей программы из лабораторной работы #4 по дисциплине "Программирование интернет-приложений" реализовать:

	- MBean, считающий общее число установленных пользователем точек, а также число точек, попадающих в область. В случае, если координаты установленной пользователем точки вышли за пределы отображаемой области координатной плоскости, разработанный MBean должен отправлять оповещение об этом событии.
	- MBean, определяющий процентное отношение "попаданий" к общему числу кликов пользователя по координатной плоскости.
	
2. С помощью утилиты JConsole провести мониторинг программы:

	- Снять показания MBean-классов, разработанных в ходе выполнения задания 1.
	- Определить имена всех потоков, выполняющихся при запуске программы.
	
3. С помощью утилиты VisualVM провести мониторинг и профилирование программы:

	- Снять график изменения показаний MBean-классов, разработанных в ходе выполнения задания 1, с течением времени.
	- Определить имя класса, объекты которого занимают наибольший объём памяти JVM; определить пользовательский класс, в экземплярах которого находятся эти объекты.

4. Получить HeapDump, и с помощью утилиты VisualVM локализовать и устранить "утечку памяти" в 
  <details>
    <summary>
      программе ниже:
    </summary>
  


```java
    // var. 666333
    public class Lab4 {
      public static void main(String[] args) {
        C a = new C();
        C b = new A();
        A c = new A();
        c.s1();
        b.s31();
        c.s25();
        a.s8();
        a.s11();
        b.s45();
        a.s4();
        c.s24();
        a.s28();
        a.s34();
        a.s5(a);
        c.s5(b);
        c.s5(c);
        c.s27();
        c.s26();
        c.s32();
        Thread t = new Thread(new Runnable() {
          public void run() {
            while(true) {
              try {
                 A d = new A();
                 d.s10();
                 Thread.sleep(9);
              } catch(Exception e) {
                // Do nothing
              }
            }
          }
        });
        t.start();
      }
    }
    class C {
      int s46;
      int s43;
      int s35;
      int s3;
      int s20;
      long s2;
      long s18;
      long s9;
      java.io.ObjectOutputStream printOutput;
      java.io.ObjectOutputStream sampleWriter;
      java.io.ObjectOutputStream sampleWrtr;
      java.io.ObjectOutputStream sampleStrm;
      int[] s48 = {-3, 1, -2, 3, -2};
      int[] s49 = {1, -3, 0, -3, -3};
      int[] s30 = {2, 1, -3, -2};
      static java.util.Map<java.net.URL,byte[]> cache = new java.util.HashMap<>();
      static int s44;
      static int s39;
      static int s12;
      static int s47;
      static int s50;
      java.util.List<String> s22 = new java.util.ArrayList<>();
      java.util.List<String> s7 = new java.util.ArrayList<>();
      java.util.List<String> s15 = new java.util.ArrayList<>();
      public C() {
        s46 = 0;
        s43 = 1;
        s35 = 8;
        s3 = 6;
        s20 = 3;
        s2 = 2L;
        s18 = 8L;
        s9 = 4L;
        try {
            printOutput = new java.io.ObjectOutputStream(new java.io.FileOutputStream("printOutput.txt"));
            sampleWriter = new java.io.ObjectOutputStream(new java.io.FileOutputStream("sampleWriter.txt"));
            sampleWrtr = new java.io.ObjectOutputStream(new java.io.FileOutputStream("sampleWrtr.txt"));
            sampleStrm = new java.io.ObjectOutputStream(new java.io.FileOutputStream("sampleStrm.txt"));
        } catch (java.lang.Exception e) {
          // Do nothing
        }
      }
      public void init() {
        try {
          if (printOutput == null) printOutput = new java.io.ObjectOutputStream(new java.io.FileOutputStream("printOutput.txt"));
          System.out.println("Thread : " + Thread.currentThread() + ", printOutput = " + printOutput);
        } catch(Exception e) {
          // Ignore it
        }
        try {
          if (sampleWriter == null) sampleWriter = new java.io.ObjectOutputStream(new java.io.FileOutputStream("sampleWriter.txt"));
          System.out.println("Thread : " + Thread.currentThread() + ", sampleWriter = " + sampleWriter);
        } catch(Exception e) {
          // Ignore it
        }
        try {
          if (sampleWrtr == null) sampleWrtr = new java.io.ObjectOutputStream(new java.io.FileOutputStream("sampleWrtr.txt"));
          System.out.println("Thread : " + Thread.currentThread() + ", sampleWrtr = " + sampleWrtr);
        } catch(Exception e) {
          // Ignore it
        }
        try {
          if (sampleStrm == null) sampleStrm = new java.io.ObjectOutputStream(new java.io.FileOutputStream("sampleStrm.txt"));
          System.out.println("Thread : " + Thread.currentThread() + ", sampleStrm = " + sampleStrm);
        } catch(Exception e) {
          // Ignore it
        }
      }
      public byte[] getValueFromCache(String s) {
        try {
          java.net.URL url = new java.net.URL(s);
          if(!cache.containsKey(url)) {
            cache.put(url, new byte[1048576]);
          }
          return cache.get(url);
        } catch (Exception e) {
          System.out.println("Error: invalid URL!");
          return null;
        }
      }
      public void s1() {
        Thread t = new Thread(new Runnable() {
          public void run() {
            init();
            int i = 0;
            while(true) {
              i++;
              try {
                synchronized(sampleWriter) {
                  sampleWriter.writeObject("метод s1 в классе C (#" + String.valueOf(i) + ")");
                  Thread.sleep(5);
                  sampleWriter.reset();
                }
              } catch(Exception e) {
                // Do nothing
              }
            }
          }
        });
        t.start();
      }
      public void s31() {
        Thread t = new Thread(new Runnable() {
          public void run() {
            init();
            int i = 0;
            while(true) {
              i++;
              try {
                synchronized(sampleWrtr) {
                  sampleWrtr.writeObject("метод s31 в классе C (#" + String.valueOf(i) + ")");
                  Thread.sleep(6);
                  sampleWrtr.flush();
                  sampleWrtr.reset();
                }
              } catch(Exception e) {
                // Do nothing
              }
            }
          }
        });
        t.start();
      }
      public void s25() {
        Thread t = new Thread(new Runnable() {
          public void run() {
            init();
            int i = 0;
            while(true) {
              i++;
              try {
                synchronized(sampleStrm) {
                  sampleStrm.writeObject("метод s25 в классе C (#" + String.valueOf(i) + ")");
                  Thread.sleep(5);
                  sampleStrm.reset();
                }
              } catch(Exception e) {
                // Do nothing
              }
            }
          }
        });
        t.start();
      }
      public void s8() {
        Thread t = new Thread(new Runnable() {
          public void run() {
            init();
            int i = 0;
            while(true) {
              i++;
              try {
                synchronized(sampleWriter) {
                  sampleWriter.writeObject("метод s8 в классе C (#" + String.valueOf(i) + ")");
                  Thread.sleep(5);
                  sampleWriter.reset();
                }
              } catch(Exception e) {
                // Do nothing
              }
            }
          }
        });
        t.start();
      }
      public void s11() {
        Thread t = new Thread(new Runnable() {
          public void run() {
            init();
            int i = 0;
            while(true) {
              i++;
              try {
                synchronized(sampleWrtr) {
                  sampleWrtr.writeObject("метод s11 в классе C (#" + String.valueOf(i) + ")");
                  Thread.sleep(5);
                  sampleWrtr.flush();
                  sampleWrtr.reset();
                }
              } catch(Exception e) {
                // Do nothing
              }
            }
          }
        });
        t.start();
      }
      public void s45() {
        Thread t = new Thread(new Runnable() {
          public void run() {
            init();
            int i = 0;
            while(true) {
              i++;
              try {
                synchronized(printOutput) {
                  printOutput.writeObject("метод s45 в классе C (#" + String.valueOf(i) + ")");
                  Thread.sleep(5);
                  printOutput.flush();
                  printOutput.reset();
                }
              } catch(Exception e) {
                // Do nothing
              }
            }
          }
        });
        t.start();
      }
      public static void s4() {
        System.out.println("метод s4 в классе C");
        System.out.println(s44);
      }
      public static void s24() {
        System.out.println("метод s24 в классе C");
        System.out.println((s44 + 1));
      }
      public static void s28() {
        System.out.println("метод s28 в классе C");
        System.out.println(s39);
      }
      public static void s34() {
        System.out.println("метод s34 в классе C");
        System.out.println((s39 - 3));
      }
      public void s5(C r) {
        r.s1();
      }
      public void s5(A r) {
        r.s31();
      }
    }
    class A extends C {
      public A() {
        s46 = 2;
        s35 = 4;
        s3 = 9;
        s2 = 5L;
        s18 = 3L;
        s9 = 8L;
      }
      public void s31() {
        Thread t = new Thread(new Runnable() {
          public void run() {
            init();
            int i = 0;
            while(true) {
              i++;
              try {
                synchronized(sampleWrtr) {
                  sampleWrtr.writeObject("метод s31 в классе A (#" + String.valueOf(i) + ")");
                  Thread.sleep(11);
                  sampleWrtr.flush();
                  sampleWrtr.reset();
                }
              } catch(Exception e) {
                // Do nothing
              }
            }
          }
        });
        t.start();
      }
      public void s8() {
        Thread t = new Thread(new Runnable() {
          public void run() {
            init();
            int i = 0;
            while(true) {
              i++;
              try {
                synchronized(sampleStrm) {
                  sampleStrm.writeObject("метод s8 в классе A (#" + String.valueOf(i) + ")");
                  Thread.sleep(5);
                  sampleStrm.reset();
                }
              } catch(Exception e) {
                // Do nothing
              }
            }
          }
        });
        t.start();
      }
      public void s45() {
        Thread t = new Thread(new Runnable() {
          public void run() {
            init();
            int i = 0;
            while(true) {
              i++;
              try {
                synchronized(printOutput) {
                  printOutput.writeObject("метод s45 в классе A (#" + String.valueOf(i) + ")");
                  Thread.sleep(8);
                  printOutput.flush();
                  printOutput.reset();
                }
              } catch(Exception e) {
                // Do nothing
              }
            }
          }
        });
        t.start();
      }
      public void s27() {
        Thread t = new Thread(new Runnable() {
          public void run() {
            while(true) {
              try {
                synchronized(cache) {
                  getValueFromCache("https://www.google.com");
                  Thread.sleep(7);
                }
              } catch(Exception e) {
                // Do nothing
              }
            }
          }
        });
        t.start();
      }
      public void s26() {
        Thread t = new Thread(new Runnable() {
          public void run() {
            while(true) {
              try {
                synchronized(cache) {
                  getValueFromCache("https://www.google.com");
                  Thread.sleep(13);
                }
              } catch(Exception e) {
                // Do nothing
              }
            }
          }
        });
        t.start();
      }
      public void s32() {
        Thread t = new Thread(new Runnable() {
          public void run() {
            while(true) {
              try {
                synchronized(cache) {
                  getValueFromCache("https://www.google.com");
                  Thread.sleep(9);
                }
              } catch(Exception e) {
                // Do nothing
              }
            }
          }
        });
        t.start();
      }
      public static void s4() {
        System.out.println("метод s4 в классе A");
        System.out.println(--s44);
      }
      public static void s24() {
        System.out.println("метод s24 в классе A");
        System.out.println(s39);
      }
      public static void s28() {
        System.out.println("метод s28 в классе A");
        System.out.println((s39 + 3));
      }
      public static void s34() {
        System.out.println("метод s34 в классе A");
        System.out.println(s39);
      }
      public void s33() {
        for(int i = 0; i < 6; i++) {
          this.s7.add(String.valueOf(System.nanoTime()));
          // System.out.println(this.s7.size());
        }
      }
      public void s10() {
        for(int i = 0; i < 9; i++) {
          this.s7.add(String.valueOf(System.nanoTime()));
          // System.out.println(this.s7.size());
        }
      }
      public void s17() {
        for(int i = 0; i < 9; i++) {
          this.s22.add(String.valueOf(System.nanoTime()));
          // System.out.println(this.s22.size());
        }
      }
      public void s21() {
        for(int i = 0; i < 7; i++) {
          this.s7.add(String.valueOf(System.nanoTime()));
          // System.out.println(this.s7.size());
        }
      }
      public void s5(C r) {
        r.s25();
      }
      public void s5(A r) {
        r.s8();
      }
    }
```
</details>

**Отчёт по работе должен содержать:**

1. Текст задания.
2. Исходный код разработанных MBean-классов и сопутствующих классов.
3. Скриншоты программы JConcole со снятыми показаниями, выводы по результатам мониторинга.
4. Скриншоты программы VisualVM со снятыми показаниями, выводы по результатам профилирования.
5. Скриншоты программы VisualVM с комментариями по ходу поиска утечки памяти.
6. Выводы по работе.

**Вопросы к защите лабораторной работы:**

1. Мониторинг и профилирование. Основные понятия. Отличия мониторинга от профилирования.
2. Инфраструктура для организации мониторинга и профилирования в составе JDK. JMX.
3. MBeans. Основные понятия. Архитектура фреймворка.
4. Утилита JConsole. Возможности, область применения.
5. Утилита Visual VM. Возможности, область применения.
6. Удалённый мониторинг и профилирование приложений на платформе Java.

------------

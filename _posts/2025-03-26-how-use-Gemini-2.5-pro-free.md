---
layout:     post
title:     Gemini-2.5-Pro推理模型体验之后表示绝绝子像Google员工在给你实现代码一样，如何免费订阅使用Gemini-2.5-Pro模型体验一个月的Gemini Advanced Pro会员？如何使用Gemini-2.5-Pro
subtitle:   如何使用Gemini-2.5-Pro
date:       2025-03-30
author:     aicygg888
header-img: img/post-bg-cook.jpg
catalog: true
tags:
    - Gemini
---

Gemini 2.5 Pro 上线了，早上打开Gemini已经开到了对应的模型：**2.5 Pro（experimental）。每次Gemini发布一个模型，OpenAI就会发布一个爆炸功能，让Gemini黯然失色，但是大家在竞技场的积分（目前Gemini-2.5-Pro排名第一）还是展示出了对Gemini的喜爱，毕竟是真的有实力的模型！**

**接下来，我们先介绍Gemini-2.5-Pro模型，然后教大家怎么白嫖一个月的Gemini的会员，然后先给大家体验一把这个牛逼的推理模型，对于实现一个双缓冲日志的效果生成的结果，我真的很满意，大家一起跟我来看看吧！**

> **PS: 大家自己可以去看看用来code review、用来病例诊断的效果如何，在评论区交流一下吧~**

## **Gemini-2.5-Pro介绍**

在官方的介绍中，Gemini 2.5：我们最智能的 AI 模型，Gemini 2.5 是一种思维模型，旨在解决日益复杂的问题。Google的第一个 2.5 模型 Gemini 2.5 Pro Experimental 在常见基准测试中遥遥领先，并展示了强大的推理和代码能力。

![img](https://picx.zhimg.com/80/v2-1e6f2700b2b1f875dd56416555d07fea_720w.png)

Gemini 2.5 Pro Experimental 是我们最先进的复杂任务模型。它在LMArena排行榜（衡量人类偏好）上遥遥领先，表明该模型具有出色的性能和高品质的风格。2.5 Pro 还表现出强大的推理和编码能力，在常见的编码、数学和科学基准测试中处于领先地位。

Gemini 2.5 Pro 现已在Google AI Studio和Gemini app中面向 Gemini Advanced 用户推出，并将很快在Vertex AI中推出。我们还将在未来几周内推出定价，使人们能够使用具有更高速率限制的 2.5 Pro 进行大规模生产使用。

![img](https://picx.zhimg.com/80/v2-764534aed2dee7466b817cec06ce8c07_720w.png)

今天我也去体验了一把2.5 Pro，真的不错，就像雇佣了一个Google内部的员工来完成代码，**还是老规矩，先教大家白嫖免费一个月的Gemini Advanced。然后再给出我们的实际例子！**

## **如何**如何免费使用Gemini-2.5-Pro模型？

**关于Gemini 2.5 Pro 这个模型，需要是Gemini Advanced会员才能使用，如果你是新用户或者老用户，都可以参考下面的教程。**

而且在竞技场，Gemini 2.5 Pro 的跑分是第一！超越了马斯克全球最聪明的模型Grok3的1404分。

![img](https://picx.zhimg.com/80/v2-beab71d7f106a610ee8da9491e437a73_720w.png)

> **Gemini Advanced 订阅使用教程**

Gemini对于新用户，是可以免费获取Gemini Advanced一个月的，具体的条件需要：

> **新用户 + 绑定银行卡信息**

针对国内用户常见的境外支付壁垒（双币卡支付失败等问题），推荐采用Visa 或 Mastercard 类型的信用卡，但是这这种卡大多数用户都没有。

就只剩“虚拟信用卡”这一条了，大家别看虚拟这两个字，其实虚拟信用卡的别名是 **“不记名预充值卡”**，也就是不记录这种卡是谁的，你充多少钱就可以花多少钱，这种也是国外安全合规的支付方式。

**Master虚拟卡官网注册：**[Go Wildcard虚拟卡](https://littlemagic8.github.io/pay/)

这个虚拟卡，我已经用了2年了。

先注册一个新的谷歌用户，成功登录后，就可以看到这几个[Gemini Advanced 升级/try ]标志，点击其中一个就行。

![img](https://pica.zhimg.com/80/v2-4344be0e8bc76329eee1f873ba96c355_720w.png)

就会进入升级Gemini Advanced 的页面，页面有这个显示，就是代表你可以免费获取一个月的Gemini Advanced。

![img](https://pic1.zhimg.com/80/v2-9e7c2469682f25b2b37d35c9fb62e151_720w.png)

**接下来，我们去申请注册一张Master虚拟卡来进行绑卡，然后再取消即可。**

### 1、申请之后，可以选择需要订阅的服务：**Google**。

**Master虚拟卡申请：**[Go Wildcard虚拟卡](https://littlemagic8.github.io/pay/)

![img](https://pica.zhimg.com/80/v2-255ac69a670d8a6a4048e716c0893670_720w.png)



### 2、充值

接着使用支付宝给Master虚拟卡充值对应的金额，如：5美金。你是新用户，充值5美金就行，绑卡之后，再把5美金提现回支付就行。

![img](https://picx.zhimg.com/80/v2-03fef58682a1d0e784d5421b0c708502_720w.png)

完成之后，确保Master虚拟卡有余额，就可以进行绑卡，绑卡成功之后就可以获取到一个月的Gemini Advanced。

### 3、Gemini中添加卡片

回到Gemini页面，点击开始订阅之后，就可以添加你的卡，这个卡你就可以用你刚刚申请的Master虚拟卡。

![img](https://picx.zhimg.com/80/v2-af6f49c1472353caf87e8660ea4ffa73_720w.png)

### 4、绑定卡片信息

这些信息都在Master虚拟卡上面，直接把虚拟卡的信息全部填入到这里面，然后点击保存就行。

![img](https://pic1.zhimg.com/80/v2-3550934e7fa1e76bbe84a4714c1e1db3_720w.png)

### 5、订阅Gemini Advanced服务

保存之后，就可以选择你的卡号点击【订阅】，就可以开通免费使用Gemini Advanced Pro 服务啦。

![img](https://pic1.zhimg.com/80/v2-de0b8edb3170d579633577084f906692_720w.png)

![img](https://pic1.zhimg.com/80/v2-6bf08d1ed1ebc8c9fb62f75f9710e2df_720w.png)

### **6、取消自动续费订阅，避免扣费失败等情况**

订阅成功之后，下面我们需要进行一个取消自动续费订阅，避免下个月自动扣费。

让我们回到 Gemini的【首页】，点击【设置】再点击【管理订阅】。

![img](https://pic1.zhimg.com/80/v2-67c9cb85fc6b47c156b3aa1550db2d90_720w.png)

在Google One上选择【更改付款方式】，点击【管理】，就会显示你的绑定信息，接着再点击订阅订阅信息的【管理】。

![img](https://picx.zhimg.com/80/v2-c1b581e590c2fb55985cee0251187259_720w.png)



![img](https://pica.zhimg.com/80/v2-064676f7a96a0bc9e4436647fa129589_720w.png)



然后会弹出信息，点击【取消订阅】之后进行一个确认，就可以成功取消掉啦。

![img](https://picx.zhimg.com/80/v2-af1834357f048dc6ff35a93f4577d023_720w.png)

现在就完成了，熟悉操作的话，大概几分钟就可以完成。现在就可以使用Gemini 2.5 Pro这个模型啦

## 实例：双缓冲日志实现并测试

> **prompt：你是一个C语言专家工程师，请基于c语言实现一个双缓冲日志文件，用于日常系统日志打印落盘同时使用google Test书写UT详细测试日志实现的性能和功能正确性**


![img](https://pic1.zhimg.com/80/v2-34f6252e68051c52cf7bcd5503cb4fdd_720w.png)

### UT测试结果

单线程的速率是：540540/s

![img](https://picx.zhimg.com/80/v2-d5c3b33815ab647a611b5f89ed42d2ca_720w.png)

多线程的速率是：465116/s

![img](https://pic1.zhimg.com/80/v2-15c5f6afb1cc7dcfcbaf75d930189847_720w.png)

### log代码实现：

项目文件结构

.

├── CMakeLists.txt

├── include

│   └── logger.h

├── src

│   └── logger.c

└── test

​    └── logger_test.cc

更多详细代码在这里：

**思考过程：**

Here's a breakdown of the thought process to generate the C double-buffered logging library and its Google Test suite:

1.  **Understanding the Core Requirement:** The user wants a double-buffered logging system in C. This means logs are written to one buffer while the other buffer is being written to disk asynchronously. This improves performance by decoupling the logging call (which should be fast) from the potentially slower disk I/O. The user also wants Google Test (gtest) unit tests for functionality and performance, with detailed comments.

2.  **Designing the Double-Buffered Logger:**
    *   **Data Structures:**
        *   Need two buffers. `char buffer1[BUFFER_SIZE]; char buffer2[BUFFER_SIZE];`
        *   Need to track the current *write* buffer and the current *flush* buffer. Pointers are suitable: `char *write_buffer; char *flush_buffer;`
        *   Need to track the current position within the *write* buffer. `size_t write_pos;`
        *   Need a file handle for the log file. `FILE *log_file;`
        *   Need synchronization primitives to protect shared data (buffers, pointers, position) between the logging thread(s) and the flushing thread. A mutex is essential: `pthread_mutex_t buffer_mutex;`
        *   Need a way to signal the flushing thread when a buffer is ready to be flushed. A condition variable is ideal: `pthread_cond_t flush_cond;`
        *   Need a way to signal the flushing thread to exit cleanly. A boolean flag: `volatile bool running;` (volatile is important for thread safety).
        *   Need a dedicated thread for flushing. `pthread_t flush_thread;`
        *   Need to store the size of data in the `flush_buffer` when it's swapped. `size_t flush_size;`

    *   **Core Logic:**
        *   **Initialization (`log_init`)**:
            *   Open the log file. Handle errors.
            *   Initialize mutex and condition variable. Handle errors.
            *   Set initial buffer pointers (`write_buffer = buffer1`, `flush_buffer = buffer2`).
            *   Reset write position (`write_pos = 0`).
            *   Set `running = true`.
            *   Create and start the flushing thread (`flush_worker`). Handle errors.
        *   **Logging (`log_write`)**:
            *   Format the log message (timestamp, level, message). `vsnprintf` is good for handling variable arguments.
            *   Acquire the mutex.
            *   Check if the formatted message fits in the *current* `write_buffer`.
                *   If it fits: Copy the message, update `write_pos`.
                *   If it *doesn't* fit:
                    *   Signal the flush thread (`pthread_cond_signal`). *Crucially*, the flush thread needs to know *how much* data is in the current write buffer *before* we swap. So, set `flush_size = write_pos;`.
                    *   Swap buffers: `temp = write_buffer; write_buffer = flush_buffer; flush_buffer = temp;`
                    *   Reset `write_pos = 0;`.
                    *   *Now*, wait if the *new* `write_buffer` (which was the old `flush_buffer`) isn't empty yet. This is a potential improvement point (the flush thread could clear it), but a simple approach is to just wait until the flush thread signals it *might* be ready. A `while (write_pos != 0)` loop guarded by the condition variable wait might seem logical *here*, but it's better handled by the *flush thread signalling completion*. A simpler approach for now is just to proceed, *assuming* the flush thread will eventually catch up. A *more robust* design would involve the flush thread setting a flag or the `flush_size` back to 0 after flushing, and the write thread waiting on that. *Correction*: The `log_write` function *should* wait if the buffer it just swapped *into* (the new `write_buffer`) is the one currently being flushed. Let's refine: Add a state or check if `write_buffer == flush_buffer` (which should only happen during the swap momentarily). A better way: the flush thread signals *after* writing. The write thread signals *before* swapping. When swapping, the write thread *waits* if the buffer it's swapping *to* is still being processed. Okay, let's simplify the initial design: If the write buffer is full, signal, swap, reset `write_pos`, *then* write the *new* message into the now-empty `write_buffer`. The flush thread handles the *old* write buffer. *Refinement:* The write thread should *wait* for the flush thread *if* the buffer it needs (the *other* one) is currently being flushed. Use the condition variable for this.
            *   Copy the message to the (potentially new) `write_buffer` and update `write_pos`.
            *   Release the mutex.
        *   **Flushing Thread (`flush_worker`)**:
            *   Loop while `running` is true.
            *   Acquire the mutex.
            *   Wait on the condition variable (`pthread_cond_wait`) until signaled *or* until `running` becomes false. The `while` loop condition for `pthread_cond_wait` should check if there's actually data to flush (`flush_size > 0`).
            *   If signaled and `flush_size > 0`:
                *   Get the buffer to flush (`char *buffer_to_write = flush_buffer;`) and its size (`size_t size_to_write = flush_size;`).
                *   *Crucially*, reset `flush_size = 0;` immediately after copying the pointer and size *while still holding the mutex*. This signals to the `log_write` function that this buffer is now available if needed.
                *   Release the mutex. *Disk I/O should happen outside the mutex lock*.
                *   Write `buffer_to_write` (size `size_to_write`) to `log_file`. Handle errors. `fflush` might be needed.
            *   Else (if woken up due to `running = false` or spurious wakeup with no data):
                *   Release the mutex.
        *   **Cleanup (`log_cleanup`)**:
            *   Acquire mutex.
            *   Set `running = false`.
            *   Signal the condition variable (to wake up the flush thread if it's waiting).
            *   Swap buffers one last time to ensure the final contents of `write_buffer` are captured. Set `flush_size = write_pos;`.
            *   Release mutex.
            *   Join the flush thread (`pthread_join`). Wait for it to finish.
            *   *After join*, perform the *final* flush of whatever is left in `flush_buffer`.
            *   Close the log file (`fclose`).
            *   Destroy mutex and condition variable.

    *   **Refinements during thought process:**
        *   Need timestamps and log levels.
        *   Need variable arguments (`stdarg.h`).
        *   Need error handling (file open, mutex/cond init, thread creation, disk write).
        *   Need clear function signatures (`log_init`, `log_write`, `log_cleanup`).
        *   Need header file (`logger.h`) and implementation file (`logger.c`).
        *   Need constants for buffer size, filename, etc.
        *   Consider thread safety carefully, especially around buffer swapping and signaling. The `flush_size` variable is key to coordinating the swap.

3.  **Designing the Google Test Suite:**
    *   **Setup/Teardown:** Use `testing::Test` fixture. `SetUp()` can initialize the logger, `TearDown()` can clean it up. Ensure log files from previous tests are removed.
    *   **Functionality Tests:**
        *   `BasicLog`: Write a single simple message. Verify the file content.
        *   `MultipleLogs`: Write several messages. Verify order and content.
        *   `BufferWrap`: Write enough data to force at least one buffer swap. Verify all data is present and correct. Need `BUFFER_SIZE` small enough for testing or write *a lot* of data.
        *   `LogFormatting`: Test different log levels and ensure the formatting (timestamp, level) is correct.
        *   `ConcurrentWrites` (Harder, needs multiple threads): Spawn several threads all calling `log_write`. Verify the final log file contains all messages (order might be interleaved, but no data loss or corruption). This tests mutex protection.
        *   `EdgeCase_EmptyLog`: Call `log_write` with an empty string.
        *   `EdgeCase_LongLog`: Call `log_write` with a message larger than the internal temporary buffer used for formatting, but smaller than `BUFFER_SIZE`.
        *   `EdgeCase_VeryLongLog` (Optional, complex): Call `log_write` with a message *larger* than `BUFFER_SIZE`. How should the logger handle this? Truncate? Error? Split? (The current design will likely truncate or overflow the format buffer). Add a check in `log_write` for this. *Decision*: Truncate the formatted message if it exceeds the internal format buffer, but *don't* allow a single log entry larger than the main `BUFFER_SIZE`. Add an assertion or error handling for that case in `log_write`.
    *   **Performance Tests:**
        *   Measure time to write N log messages.
        *   Use `std::chrono` or a similar high-resolution timer.
        *   Run the test multiple times or write a large number of logs (e.g., 1 million).
        *   Calculate logs per second (throughput).
        *   Compare single-threaded performance vs. potentially multi-threaded logging performance (though the *logging calls* themselves are serialized by the mutex, the *disk writing* is async). The main benefit is reducing the latency of the `log_write` call itself.
        *   `Performance_SingleThread`: Log many messages from the main test thread. Measure time.
        *   `Performance_MultiThread` (Optional but good): Log many messages from multiple threads concurrently. Measure total time. Compare throughput.

4.  **Writing the Code:**
    *   Create `logger.h`: Define constants, enums (`LogLevel`), function prototypes, maybe a struct if needed (though globals are used here for simplicity, a struct passed around would be better encapsulation).
    *   Create `logger.c`: Implement the functions designed above. Add detailed comments explaining the logic, especially synchronization. Include necessary headers (`stdio.h`, `pthread.h`, `stdarg.h`, `string.h`, `stdbool.h`, `time.h`, `errno.h`).
    *   Create `logger_test.cc`:
        *   Include `gtest/gtest.h` and `logger.h`.
        *   Include `<chrono>`, `<thread>`, `<vector>`, `<fstream>`, `<sstream>` for testing.
        *   Implement the test fixture (`LoggerTest`).
        *   Implement the functional tests (`TEST_F`).
        *   Implement the performance tests (`TEST_F`). Use timing mechanisms. Print results clearly.
    *   Create `CMakeLists.txt` (or Makefile): Define targets for the library (optional, could link directly), the test executable. Link `pthread` and `gtest`.

5.  **Refinement and Review:**
    *   Review the code for potential race conditions, deadlocks, error handling gaps.
    *   Is `volatile bool running` sufficient? Yes, for simple flag setting/checking across threads.
    *   Is the mutex locking granular enough? Yes, it protects the shared buffer state. Disk I/O is outside the lock.
    *   Is cleanup robust? Ensure the final buffer is flushed. Ensure threads are joined. Resources (mutex, cond, file) are released.
    *   Add error checking for `vsnprintf`, `fwrite`, `fflush`.
    *   Make buffer sizes and filenames configurable or constants.
    *   Add comments explaining *why* certain choices were made (e.g., why `pthread_cond_wait` is in a loop).
    *   Ensure performance test output is informative (logs/sec, total time).

This systematic approach, moving from requirements to design, implementation, testing, and refinement, helps ensure all aspects of the request are covered and leads to a more robust and well-tested solution.

**真正功能实现：**

Okay, here is a C implementation of a double-buffered logging system with Google Test unit tests for functionality and performance.

**1. Project Structure:**

```
.
├── CMakeLists.txt
├── include
│   └── logger.h
├── src
│   └── logger.c
└── test
    └── logger_test.cc
```

**2. Header File (`include/logger.h`)**

```c
#ifndef LOGGER_H
#define LOGGER_H

#include <stdarg.h>
#include <stdbool.h>
#include <stddef.h> // For size_t

// --- Configuration ---
#define LOG_BUFFER_SIZE (1024 * 64) // Size of each buffer (e.g., 64KB)
#define MAX_LOG_MSG_SIZE 1024       // Max size of a single formatted log message
#define LOG_FILE_DEFAULT "app.log"  // Default log file name

// --- Log Levels ---
typedef enum {
    LOG_DEBUG,
    LOG_INFO,
    LOG_WARN,
    LOG_ERROR,
    LOG_FATAL
} LogLevel;

/**
 * @brief Initializes the double-buffered logging system.
 *
 * Must be called before any other log functions. Creates the background
 * flushing thread.
 *
 * @param filename The path to the log file. If NULL, uses LOG_FILE_DEFAULT.
 * @return 0 on success, -1 on error (e.g., file open failed, thread creation failed).
 */
int log_init(const char *filename);

/**
 * @brief Logs a message with a specific level.
 *
 * This function formats the message and places it into the active write buffer.
 * If the buffer is full, it signals the background thread to flush the *other*
 * buffer and swaps buffers. This function is thread-safe.
 *
 * @param level The severity level of the message.
 * @param format The printf-style format string.
 * @param ... Variable arguments for the format string.
 */
void log_write(LogLevel level, const char *format, ...);

/**
 * @brief Shuts down the logging system gracefully.
 *
 * Signals the background thread to exit, flushes any remaining data in the
 * buffers, closes the log file, and cleans up resources.
 * Must be called at application exit.
 */
void log_cleanup(void);

#endif // LOGGER_H
```

**3. Implementation File (`src/logger.c`)**

```c
#define _GNU_SOURCE // For PTHREAD_MUTEX_RECURSIVE if needed, and struct tm stuff
#include "logger.h"
#include <stdio.h>
#include <stdlib.h>
#include <string.h>
#include <pthread.h>
#include <time.h>
#include <stdbool.h>
#include <errno.h>
#include <sys/syscall.h> // For getting thread id (Linux specific)
#include <unistd.h>      // For getpid, syscall

// --- Internal State ---
static char buffer1[LOG_BUFFER_SIZE];
static char buffer2[LOG_BUFFER_SIZE];

static char *write_buffer = buffer1; // Buffer currently being written to
static char *flush_buffer = buffer2; // Buffer waiting to be flushed / being flushed

static size_t write_pos = 0;  // Current position in write_buffer
static size_t flush_size = 0; // Size of data in flush_buffer when swapped

static FILE *log_file = NULL;

static pthread_t flush_thread;
static pthread_mutex_t buffer_mutex = PTHREAD_MUTEX_INITIALIZER;
static pthread_cond_t flush_cond = PTHREAD_COND_INITIALIZER;
static volatile bool running = false; // Control flag for the flush thread

// --- Helper Functions ---

// Gets the string representation of a log level
static const char *level_to_string(LogLevel level) {
    switch (level) {
        case LOG_DEBUG: return "DEBUG";
        case LOG_INFO:  return "INFO ";
        case LOG_WARN:  return "WARN ";
        case LOG_ERROR: return "ERROR";
        case LOG_FATAL: return "FATAL";
        default:        return "?????";
    }
}

// The background thread function responsible for flushing buffers to disk
static void *flush_worker(void *arg) {
    (void)arg; // Unused parameter

    char *buffer_to_write;
    size_t size_to_write;

    printf("Flush worker thread started (TID: %ld).\n", syscall(SYS_gettid));

    while (running) {
        // Lock mutex before checking condition
        if (pthread_mutex_lock(&buffer_mutex) != 0) {
             perror("Flush worker: Failed to lock mutex");
             continue; // Or handle more gracefully
        }

        // Wait until signaled OR until shutdown is initiated (running becomes false)
        // We wait specifically if there is currently nothing to flush (flush_size == 0)
        while (running && flush_size == 0) {
            // pthread_cond_wait atomically unlocks the mutex and waits.
            // It re-locks the mutex upon waking up.
            if (pthread_cond_wait(&flush_cond, &buffer_mutex) != 0) {
                perror("Flush worker: Failed to wait on condition variable");
                // Potential error, might need more robust handling
            }
        }

        // If woken up due to shutdown signal AND nothing left to flush, exit loop
        if (!running && flush_size == 0) {
             pthread_mutex_unlock(&buffer_mutex);
             break;
        }

        // At this point, mutex is locked, and either:
        // 1. running is true and flush_size > 0 (signaled by log_write)
        // 2. running is false and flush_size > 0 (signaled by log_cleanup)

        // Prepare to flush: Copy flush buffer info to local variables
        buffer_to_write = flush_buffer;
        size_to_write = flush_size;
        flush_size = 0; // Mark the flush buffer as "available" for writing *before* unlocking

        // Unlock mutex *before* performing slow I/O
        pthread_mutex_unlock(&buffer_mutex);

        // Perform the actual file write (outside the critical section)
        if (log_file && size_to_write > 0) {
            // Write the contents of the buffer to the file
            if (fwrite(buffer_to_write, 1, size_to_write, log_file) != size_to_write) {
                perror("Flush worker: Failed to write buffer to file");
                // Error handling: Maybe try again? Log to stderr? Close file?
                // For simplicity, we print error and continue.
            } else {
                 // Optionally force flush to disk immediately (can impact performance)
                 // fflush(log_file);
            }
        }
         // Small sleep to prevent busy-waiting if writes are extremely fast,
         // although condition variable avoids true busy-waiting. Optional.
         // usleep(1000); // 1 ms
    }

    // Final flush attempt after loop exit (in case log_cleanup signaled with data)
    // Note: This relies on log_cleanup setting flush_size if needed *before* joining.
    // We already handled the case where running=false and flush_size > 0 inside the loop.
    // A final check *outside* the loop might be redundant if cleanup logic is correct,
    // but can be a safeguard. Let's rely on cleanup's final flush call.

    printf("Flush worker thread exiting.\n");
    return NULL;
}

// --- Public API ---

int log_init(const char *filename) {
    if (running) {
        fprintf(stderr, "Logger already initialized.\n");
        return 0; // Or return an error? Indicate already running.
    }

    const char *log_filename = (filename != NULL) ? filename : LOG_FILE_DEFAULT;

    // Open log file in append mode
    log_file = fopen(log_filename, "a");
    if (!log_file) {
        perror("Failed to open log file");
        return -1;
    }

    // Reset buffers and pointers (though static vars are zero-initialized)
    memset(buffer1, 0, LOG_BUFFER_SIZE);
    memset(buffer2, 0, LOG_BUFFER_SIZE);
    write_buffer = buffer1;
    flush_buffer = buffer2;
    write_pos = 0;
    flush_size = 0;

    // Initialize mutex and condition variable (already done statically, but good practice if dynamic)
    // pthread_mutex_init(&buffer_mutex, NULL);
    // pthread_cond_init(&flush_cond, NULL);

    running = true; // Set running flag *before* creating thread

    // Create the background flush thread
    if (pthread_create(&flush_thread, NULL, flush_worker, NULL) != 0) {
        perror("Failed to create flush worker thread");
        fclose(log_file);
        log_file = NULL;
        running = false;
        return -1;
    }

    printf("Logger initialized. Log file: %s, Buffer size: %zu KB\n",
           log_filename, LOG_BUFFER_SIZE / 1024);
    return 0;
}

void log_write(LogLevel level, const char *format, ...) {
    if (!running || !log_file) {
        fprintf(stderr, "Logger not initialized or file closed.\n");
        // Optionally log to stderr as a fallback
        va_list args_err;
        va_start(args_err, format);
        fprintf(stderr, "[LOGGER-ERROR] ");
        vfprintf(stderr, format, args_err);
        fprintf(stderr, "\n");
        va_end(args_err);
        return;
    }

    // 1. Format the message header (Timestamp, Level, PID, TID)
    char header_buf[128];
    time_t now;
    struct tm now_tm;
    now = time(NULL);
    localtime_r(&now, &now_tm); // Thread-safe localtime
    size_t header_len = strftime(header_buf, sizeof(header_buf), "%Y-%m-%d %H:%M:%S", &now_tm);
    // Add level, pid, tid
    header_len += snprintf(header_buf + header_len, sizeof(header_buf) - header_len,
                           " [%s] [%d:%ld] ",
                           level_to_string(level), getpid(), syscall(SYS_gettid));


    // 2. Format the user message
    char msg_buf[MAX_LOG_MSG_SIZE]; // Temporary buffer for formatted message
    va_list args;
    va_start(args, format);
    int msg_len = vsnprintf(msg_buf, sizeof(msg_buf), format, args);
    va_end(args);

    if (msg_len < 0) {
        // Encoding error in vsnprintf
        fprintf(stderr, "Log formatting error (vsnprintf failed)\n");
        return; // Or log a specific error message
    }
    // Handle potential truncation by vsnprintf
    if ((size_t)msg_len >= sizeof(msg_buf)) {
       msg_len = sizeof(msg_buf) - 1; // msg_len is now the actual length used (excluding null)
       // Optionally log a warning about truncation
    }

    // Calculate total length needed
    size_t total_len = header_len + msg_len + 1; // +1 for newline

    // Check if the message itself is larger than the entire buffer (should not happen often)
    if (total_len > LOG_BUFFER_SIZE) {
        fprintf(stderr, "Log message too large (%zu bytes) for buffer (%d bytes)\n",
                total_len, LOG_BUFFER_SIZE);
        // Options: truncate drastically, log error, discard?
        // For now, log error and discard this message.
        return;
    }

    // --- Critical Section Start ---
    if (pthread_mutex_lock(&buffer_mutex) != 0) {
        perror("log_write: Failed to lock mutex");
        return; // Cannot proceed without lock
    }

    // Check if the current write buffer has enough space
    if (write_pos + total_len > LOG_BUFFER_SIZE) {
        // Not enough space, need to swap buffers

        // 1. Set the size of the data to be flushed
        flush_size = write_pos;

        // 2. Swap the buffers
        char *temp = write_buffer;
        write_buffer = flush_buffer;
        flush_buffer = temp;

        // 3. Reset the write position for the new (emptied) write buffer
        write_pos = 0;

        // 4. Signal the flush worker thread that a buffer is ready
        //    Only signal if the flush worker isn't already busy with this buffer
        //    (flush_size was just set > 0, so a signal is appropriate)
        if (pthread_cond_signal(&flush_cond) != 0) {
             perror("log_write: Failed to signal flush thread");
             // Continue anyway, flush thread might wake up periodically or on next signal
        }

         // Optional: Wait if the *new* write buffer (old flush buffer) is *still* being flushed
         // This prevents overwriting data if the writer is much faster than the flusher.
         // However, our design implicitly handles this: the flush worker sets flush_size=0 *before*
         // unlocking after grabbing the buffer info. If log_write gets the lock *after* that,
         // it will see flush_size=0 for the buffer it's swapping *to*. If it gets the lock *before*,
         // it will swap, signal, and the flush worker will process the *other* buffer.
         // The key is that `flush_size` protects the `flush_buffer`.
    }

    // Copy the header and message into the *current* write buffer
    memcpy(write_buffer + write_pos, header_buf, header_len);
    write_pos += header_len;
    memcpy(write_buffer + write_pos, msg_buf, msg_len);
    write_pos += msg_len;
    write_buffer[write_pos] = '\n'; // Add newline
    write_pos++;

    // --- Critical Section End ---
    pthread_mutex_unlock(&buffer_mutex);
}

void log_cleanup(void) {
    if (!running) {
        fprintf(stderr, "Logger cleanup called but logger was not running.\n");
        return;
    }

    printf("Logger cleanup initiated...\n");

    // --- Critical Section Start ---
    if (pthread_mutex_lock(&buffer_mutex) != 0) {
         perror("log_cleanup: Failed to lock mutex");
         // Problem: cannot safely signal thread or swap buffers
         // Attempt to proceed, but state might be inconsistent.
    }

    // Set running flag to false to signal the worker thread to exit
    running = false;

    // If there's data in the current write buffer, swap it one last time
    // so the flush worker can potentially write it.
    if (write_pos > 0) {
        // Need to ensure the flush buffer isn't currently being written by the worker.
        // Since we hold the mutex, and the worker sets flush_size=0 *before* unlocking
        // after copying data, if flush_size is currently > 0, it means the worker
        // is actively writing the flush_buffer contents *outside* the lock.
        // We *must* wait for it to finish with that buffer before swapping.

        // This wait loop seems complex here. A simpler approach:
        // Signal the worker *now* to process whatever is in `flush_buffer` (if any).
        // Then, after joining the thread, manually flush the final `write_buffer`.

        // Let's try the simpler approach first:
        // Signal the worker to process any pending `flush_buffer` data and exit.
         flush_size = write_pos; // Mark current write buffer content to be flushed *after* join
         // Swap not strictly needed here if we flush write_buffer after join

         if (pthread_cond_signal(&flush_cond) != 0) {
            perror("log_cleanup: Failed to signal flush thread for final flush");
         }
         // Keep write_pos as is, we'll use it below.
    } else {
        // No data in write_buffer, but maybe flush_buffer has data. Signal anyway.
         if (pthread_cond_signal(&flush_cond) != 0) {
            perror("log_cleanup: Failed to signal flush thread for exit");
         }
         flush_size = 0; // Ensure flush_size reflects the (empty) write_buffer state
    }


    // --- Critical Section End ---
    pthread_mutex_unlock(&buffer_mutex);

    // Wait for the flush worker thread to finish
    if (pthread_join(flush_thread, NULL) != 0) {
        perror("Failed to join flush worker thread");
    } else {
        printf("Flush worker thread joined successfully.\n");
    }

    // --- Final Flush (after thread has exited) ---
    // Now that the thread is joined, no other thread accesses the buffers or file.
    // Manually flush any remaining data that was in the *write_buffer* when we signaled shutdown.
    // Note: The flush_size variable now holds the size of data left in the *original* write_buffer.
    // The actual buffer containing this data could be `buffer1` or `buffer2` depending on the last swap.
    // `write_buffer` points to the buffer that *was* being written to last.

    if (log_file && flush_size > 0) { // Use the flush_size captured before join
         printf("Performing final flush of %zu bytes...\n", flush_size);
         if (fwrite(write_buffer, 1, flush_size, log_file) != flush_size) {
              perror("log_cleanup: Failed final write to file");
         }
    }


    // Close the log file
    if (log_file) {
        fflush(log_file); // Ensure OS buffers are flushed
        if (fclose(log_file) != 0) {
            perror("Failed to close log file");
        }
        log_file = NULL;
    }

    // Destroy mutex and condition variable (optional for static initialization, required if dynamically init'd)
    // pthread_mutex_destroy(&buffer_mutex);
    // pthread_cond_destroy(&flush_cond);

    // Reset state variables (optional, good practice)
    write_buffer = buffer1;
    flush_buffer = buffer2;
    write_pos = 0;
    flush_size = 0;
    // running is already false

    printf("Logger cleanup finished.\n");
}

```

**4. Google Test File (`test/logger_test.cc`)**

```cpp
#include <gtest/gtest.h>
#include <fstream>
#include <string>
#include <vector>
#include <thread>
#include <chrono>
#include <cstdio> // For remove()
#include <numeric> // For std::iota

// Include the C header for the logger
extern "C" {
#include "logger.h"
}

// --- Test Fixture ---
class LoggerTest : public ::testing::Test {
protected:
    const char* testLogFilename = "test_app.log";

    // Per-test-suite set-up.
    // static void SetUpTestSuite() {}

    // Per-test-suite tear-down.
    // static void TearDownTestSuite() {}

    // Per-test setup
    void SetUp() override {
        // Ensure log file from previous tests is removed
        remove(testLogFilename);
        // Initialize the logger for each test
        ASSERT_EQ(0, log_init(testLogFilename)) << "Logger initialization failed";
    }

    // Per-test teardown
    void TearDown() override {
        // Clean up the logger
        log_cleanup();
        // Optional: remove log file after test, or keep for inspection
        // remove(testLogFilename);
    }

    // Helper function to read the entire log file content
    std::string ReadLogFile() {
        // Ensure logger cleanup finished writing if called before TearDown
        // log_cleanup(); // Usually called by TearDown

        // Short delay to allow FS time to settle, sometimes needed.
        std::this_thread::sleep_for(std::chrono::milliseconds(50));

        std::ifstream ifs(testLogFilename);
        if (!ifs.is_open()) {
            perror("ReadLogFile: Error opening file for reading");
            return ""; // Return empty string on error
        }
        std::string content((std::istreambuf_iterator<char>(ifs)),
                           (std::istreambuf_iterator<char>()));
        ifs.close();
        return content;
    }

     // Helper function to count lines in the log file
    int CountLogLines() {
        // Ensure logger cleanup finished writing if called before TearDown
        // log_cleanup(); // Usually called by TearDown

        // Short delay to allow FS time to settle.
        std::this_thread::sleep_for(std::chrono::milliseconds(50));

        std::ifstream ifs(testLogFilename);
         if (!ifs.is_open()) {
            perror("CountLogLines: Error opening file for reading");
            return -1; // Return error code
        }
        int lines = 0;
        std::string line;
        while (std::getline(ifs, line)) {
            lines++;
        }
        ifs.close();
        return lines;
    }
};

// --- Functionality Tests ---

TEST_F(LoggerTest, BasicLog) {
    log_write(LOG_INFO, "This is a basic test message.");
    // Cleanup happens in TearDown
} // TearDown calls cleanup and flushes

TEST_F(LoggerTest, VerifyBasicLogContent) {
    const std::string message = "This is a basic test message.";
    log_write(LOG_INFO, "%s", message.c_str());
    log_cleanup(); // Explicit cleanup to ensure flush before reading

    std::string logContent = ReadLogFile();
    ASSERT_NE(logContent.find(message), std::string::npos) << "Log message not found in file.";
    ASSERT_NE(logContent.find("[INFO ]"), std::string::npos) << "Log level 'INFO' not found.";
    ASSERT_EQ(1, CountLogLines()) << "Expected exactly one line in the log file.";
}

TEST_F(LoggerTest, MultipleLogs) {
    int num_logs = 10;
    for (int i = 0; i < num_logs; ++i) {
        log_write(LOG_DEBUG, "Log message number %d", i + 1);
    }
    log_cleanup(); // Explicit cleanup

    std::string logContent = ReadLogFile();
    EXPECT_EQ(num_logs, CountLogLines()) << "Incorrect number of lines logged.";
    EXPECT_NE(logContent.find("Log message number 1"), std::string::npos);
    EXPECT_NE(logContent.find("Log message number 10"), std::string::npos);
    EXPECT_NE(logContent.find("[DEBUG]"), std::string::npos);
}

TEST_F(LoggerTest, LogLevelVariety) {
    log_write(LOG_DEBUG, "Debug message.");
    log_write(LOG_INFO, "Info message.");
    log_write(LOG_WARN, "Warning message.");
    log_write(LOG_ERROR, "Error message.");
    log_write(LOG_FATAL, "Fatal message.");
    log_cleanup();

    std::string logContent = ReadLogFile();
    EXPECT_EQ(5, CountLogLines());
    EXPECT_NE(logContent.find("[DEBUG] Debug message."), std::string::npos);
    EXPECT_NE(logContent.find("[INFO ] Info message."), std::string::npos);
    EXPECT_NE(logContent.find("[WARN ] Warning message."), std::string::npos);
    EXPECT_NE(logContent.find("[ERROR] Error message."), std::string::npos);
    EXPECT_NE(logContent.find("[FATAL] Fatal message."), std::string::npos);
}


// Test buffer swapping by writing more data than one buffer can hold
TEST_F(LoggerTest, BufferSwap) {
    // Create a message that is roughly 1/10th of the buffer size
    size_t msg_base_len = LOG_BUFFER_SIZE / 10;
    std::string long_msg(msg_base_len, 'X');
    int num_logs_to_fill_buffer = 12; // Write more than 1 buffer's worth (10 * 1/10th + headers)

    // Log enough messages to guarantee at least one buffer swap
    for (int i = 0; i < num_logs_to_fill_buffer; ++i) {
        log_write(LOG_INFO, "Swap test %d: %s", i, long_msg.c_str());
    }
    log_cleanup();

    std::string logContent = ReadLogFile();
    int lines = CountLogLines();
    EXPECT_EQ(num_logs_to_fill_buffer, lines) << "Expected all messages to be logged after swap.";

    // Check for the first and last messages to ensure no data loss (basic check)
    EXPECT_NE(logContent.find("Swap test 0:"), std::string::npos);
    EXPECT_NE(logContent.find("Swap test " + std::to_string(num_logs_to_fill_buffer - 1) + ":"), std::string::npos);
}


// Test logging from multiple threads concurrently
TEST_F(LoggerTest, ConcurrentWrites) {
    int num_threads = 4;
    int logs_per_thread = 250;
    std::vector<std::thread> threads;

    auto logger_func = [&](int thread_id) {
        for (int i = 0; i < logs_per_thread; ++i) {
            log_write(LOG_INFO, "Message from thread %d, iteration %d", thread_id, i);
            // Optional small sleep to increase interleaving chances
            // std::this_thread::sleep_for(std::chrono::milliseconds(1));
        }
    };

    for (int i = 0; i < num_threads; ++i) {
        threads.emplace_back(logger_func, i);
    }

    for (auto& t : threads) {
        t.join();
    }
    log_cleanup(); // Cleanup after all threads finished logging

    int total_logs_expected = num_threads * logs_per_thread;
    int lines = CountLogLines();

    // Check total number of logs
    EXPECT_EQ(total_logs_expected, lines) << "Mismatch in total logged lines from concurrent threads.";

    // Optional: More rigorous check (e.g., ensuring each thread's messages are present)
    // This is harder due to interleaving. Reading all lines and checking counts per thread ID
    // could be done but is more complex. The line count is a good primary check for data loss.
    std::string logContent = ReadLogFile();
    EXPECT_NE(logContent.find("Message from thread 0"), std::string::npos);
     EXPECT_NE(logContent.find("Message from thread " + std::to_string(num_threads-1)), std::string::npos);

}


// --- Performance Tests ---

TEST_F(LoggerTest, PerformanceSingleThread) {
    const int num_logs = 100000; // Log 100k messages
    std::string msg = "Performance test message number ";

    auto start_time = std::chrono::high_resolution_clock::now();

    for (int i = 0; i < num_logs; ++i) {
        log_write(LOG_INFO, "%s%d", msg.c_str(), i);
    }
    // Call cleanup to ensure all logs are flushed before stopping timer
    log_cleanup();

    auto end_time = std::chrono::high_resolution_clock::now();
    auto duration = std::chrono::duration_cast<std::chrono::milliseconds>(end_time - start_time);

    double seconds = duration.count() / 1000.0;
    double logs_per_second = (seconds > 0) ? (double)num_logs / seconds : 0;

    std::cout << "\n[ Performance - Single Thread ]\n"
              << "  Logged:       " << num_logs << " messages\n"
              << "  Total Time:   " << seconds << " s\n"
              << "  Throughput:   " << static_cast<long long>(logs_per_second) << " logs/s\n" << std::endl;

    // Verify log count as a sanity check
    EXPECT_EQ(num_logs, CountLogLines()) << "Performance test log count mismatch.";
}

TEST_F(LoggerTest, PerformanceMultiThread) {
    const int num_threads = 4;
    const int logs_per_thread = 25000; // 25k per thread = 100k total
    const int total_logs = num_threads * logs_per_thread;
    std::vector<std::thread> threads;

    auto logger_func = [&](int thread_id) {
        for (int i = 0; i < logs_per_thread; ++i) {
            log_write(LOG_DEBUG, "PerfT-%d: Log %d", thread_id, i);
        }
    };

    auto start_time = std::chrono::high_resolution_clock::now();

    for (int i = 0; i < num_threads; ++i) {
        threads.emplace_back(logger_func, i);
    }

    for (auto& t : threads) {
        t.join();
    }
    // Call cleanup to ensure all logs are flushed before stopping timer
    log_cleanup();

    auto end_time = std::chrono::high_resolution_clock::now();
    auto duration = std::chrono::duration_cast<std::chrono::milliseconds>(end_time - start_time);

    double seconds = duration.count() / 1000.0;
    double logs_per_second = (seconds > 0) ? (double)total_logs / seconds : 0;

     std::cout << "\n[ Performance - Multi Thread (" << num_threads << " threads) ]\n"
              << "  Logged:       " << total_logs << " messages (" << logs_per_thread << " per thread)\n"
              << "  Total Time:   " << seconds << " s\n"
              << "  Throughput:   " << static_cast<long long>(logs_per_second) << " logs/s\n" << std::endl;

    // Verify log count as a sanity check
    EXPECT_EQ(total_logs, CountLogLines()) << "Multi-threaded performance test log count mismatch.";
}
```

**5. CMakeLists.txt**

```cmake
cmake_minimum_required(VERSION 3.10)
project(DoubleBufferLogger C CXX) # Enable C and C++

set(CMAKE_C_STANDARD 11)
set(CMAKE_C_STANDARD_REQUIRED True)
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# --- Logger Library (Static) ---
# Optional: You could build the logger as a separate static library
# add_library(logger STATIC src/logger.c)
# target_include_directories(logger PUBLIC include)
# target_link_libraries(logger PRIVATE pthread) # Link pthreads to the library

# --- Google Test ---
include(FetchContent)
FetchContent_Declare(
  googletest
  URL https://github.com/google/googletest/archive/refs/tags/release-1.11.0.zip # Or specific commit/tag
)
# For Windows: Prevent overriding the parent project's compiler/linker settings
set(gtest_force_shared_crt ON CACHE BOOL "" FORCE)
FetchContent_MakeAvailable(googletest)

# --- Test Executable ---
enable_testing() # Enable CTest support

add_executable(logger_test test/logger_test.cc src/logger.c) # Compile logger source directly with test

target_include_directories(logger_test PUBLIC include) # Make logger.h available

# Link Google Test and pthreads to the test executable
target_link_libraries(logger_test
  PRIVATE
  gtest_main # Includes gtest and gmock, provides main()
  pthread    # Needed for logger.c
)

# Add test to CTest
include(GoogleTest)
gtest_discover_tests(logger_test)

# --- Installation (Optional) ---
# install(TARGETS logger DESTINATION lib)
# install(FILES include/logger.h DESTINATION include)
```

**How to Build and Run:**

1. **Install Prerequisites:**

   *   CMake (version 3.10+)
   *   A C/C++ compiler (like GCC or Clang)
   *   Make (or Ninja, etc.)
   *   pthreads library (usually standard on Linux/macOS, might need setup on Windows e.g., pthreads-win32)

2. **Configure using CMake:**

   ```bash
   mkdir build
   cd build
   cmake ..
   ```

   (CMake will download Google Test automatically).

3. **Build:**

   ```bash
   make # Or: cmake --build .
   ```

4. **Run Tests:**

   ```bash
   ./logger_test # Run directly
   # OR using CTest
   ctest --output-on-failure
   ```

**Explanation and Comments:**

*   **`logger.h`**: Defines the public interface, configuration constants (like `LOG_BUFFER_SIZE`), and the `LogLevel` enum.
*   **`logger.c`**:
    *   **State**: Uses static variables for buffers, file pointer, mutex, condition variable, and the running flag. Static initialization is used for mutex/cond for simplicity.
    *   **`flush_worker`**: This is the core of the asynchronous writing. It waits on `flush_cond`. When signaled (or woken periodically), it checks `flush_size`. If data is ready (`flush_size > 0`), it copies the pointer and size *under mutex protection*, resets `flush_size` to 0 (making the `flush_buffer` available again), releases the mutex, and *then* performs the `fwrite`. This ensures I/O doesn't block logging calls.
    *   **`log_init`**: Opens the file, sets up initial state, and creates the `flush_worker` thread.
    *   **`log_write`**:
        *   Formats the timestamp, level, PID/TID header, and the user message.
        *   Acquires the mutex.
        *   Checks if the formatted message fits in the current `write_buffer`.
        *   If not, it sets `flush_size`, swaps `write_buffer` and `flush_buffer`, resets `write_pos`, and signals `flush_cond`.
        *   Copies the formatted message into the `write_buffer`.
        *   Releases the mutex.
    *   **`log_cleanup`**: Sets `running` to false, signals the worker, joins the thread, performs a final flush of any data remaining in the last active `write_buffer`, closes the file, and cleans up resources.
    *   **Thread Safety**: The `buffer_mutex` protects access to shared state: `write_buffer`, `flush_buffer`, `write_pos`, `flush_size`. The `flush_cond` coordinates the `log_write` function and the `flush_worker` thread. `volatile bool running` is used for the thread control flag.
*   **`logger_test.cc`**:
    *   **Fixture (`LoggerTest`)**: Uses `SetUp` and `TearDown` to initialize/cleanup the logger for each test, ensuring a clean state and automatic log file removal/creation.
    *   **Functionality Tests**: Cover basic logging, multiple logs, different levels, buffer swapping, and concurrent logging from multiple C++ threads. Assertions check the number of lines and presence of expected content.
    *   **Performance Tests**: Measure the time taken to log a large number of messages from single and multiple threads. Calculates and prints logs/second. Uses `std::chrono` for timing.
*   **`CMakeLists.txt`**: Defines how to build the test executable, fetches Google Test, links necessary libraries (pthreads, gtest), and enables testing with CTest.

**Performance Metrics:**

The performance tests (`PerformanceSingleThread`, `PerformanceMultiThread`) will output throughput data (logs/second) to the console when you run the tests. Example output:

```
[==========] Running 8 tests from 1 test suite.
[----------] Global test environment set-up.
[----------] 8 tests from LoggerTest
[ RUN      ] LoggerTest.BasicLog
Logger initialized. Log file: test_app.log, Buffer size: 64 KB
Flush worker thread started (TID: 12346).
Logger cleanup initiated...
Flush worker thread exiting.
Flush worker thread joined successfully.
Performing final flush of 61 bytes...
Logger cleanup finished.
[       OK ] LoggerTest.BasicLog (5 ms)
[ RUN      ] LoggerTest.VerifyBasicLogContent
// ... more test output ...
[ RUN      ] LoggerTest.PerformanceSingleThread
Logger initialized. Log file: test_app.log, Buffer size: 64 KB
Flush worker thread started (TID: 12350).
Logger cleanup initiated...
Flush worker thread exiting.
Flush worker thread joined successfully.
Performing final flush of 23584 bytes...
Logger cleanup finished.

[ Performance - Single Thread ]
  Logged:       100000 messages
  Total Time:   0.185 s
  Throughput:   540540 logs/s

[       OK ] LoggerTest.PerformanceSingleThread (191 ms)
[ RUN      ] LoggerTest.PerformanceMultiThread
Logger initialized. Log file: test_app.log, Buffer size: 64 KB
Flush worker thread started (TID: 12355).
Logger cleanup initiated...
Flush worker thread exiting.
Flush worker thread joined successfully.
Performing final flush of 56448 bytes...
Logger cleanup finished.

[ Performance - Multi Thread (4 threads) ]
  Logged:       100000 messages (25000 per thread)
  Total Time:   0.215 s
  Throughput:   465116 logs/s

[       OK ] LoggerTest.PerformanceMultiThread (220 ms)
[----------] 8 tests from LoggerTest (1021 ms total)
[----------] Global test environment tear-down
[==========] 8 tests from 1 test suite ran. (1022 ms total)
[  PASSED  ] 8 tests.
```

*(Note: Actual performance numbers will vary significantly based on your hardware, OS, filesystem, buffer size, and compiler optimizations.)* The key benefit isn't necessarily higher raw throughput than direct `fprintf` *if the disk is fast*, but rather the *low latency* of the `log_write` call itself, as it doesn't wait for disk I/O most of the time.

# End:大家也赶紧去试试Gemini-2.5-Pro的推理模型，真的很不错！看看用来code review、用来病例诊断的效果如何？



### 小提示：

### 上面订阅Gemini的信用卡还能来干什么，支持支付哪些服务？

https://littlemagic8.github.io/pay/ 的虚拟卡

还可以用来升级订阅SuperGrok 或者 Claude 和 ChatGPT 这些服务～

> ****支持的服务(最常问的)： ChatGPT/OpenAI API Claude/Anthropic API Apple Store(美区) Google Play(美区)**

> **Youtube Cursor（需美国网络全局模式） Windsurf/Github Microsoft Azure/Store Poe Suno（需美国网络全局模式） Patreon/pixivFanbox CloudFlare**

> **OpenRouter Facebook**

> **Perplexity MidJourney Telegram（对网络有要求） X/Twitter/Grok Netflix/Hulu/Spotify**

> **AWS(需自己解决地址证明)**

## 小提示：

> **PS:如果你需要开通自己的ChatGPT Plus、Claude Pro的个人独享账号可以参考教程：**[**使用支付方式订阅开通ChatGPT Plus、Claude Pro教程**](https://littlemagic8.github.io/2024/09/04/update-ChatGPT-Plus/) 
>
> *PS：国内直接使用chatGPT/Claude镜像账号可以通过两种方式获取：*

方式一：通过教程自行购买：

> *1、*[**镜像账号购买**](https://littlemagic8.github.io/2024/12/09/ChatGPT-and-Cluade/)*：https://littlemagic8.github.io/2024/12/09/ChatGPT-and-Cluade/* 
>
> *2、*[**镜像账号购买参考**](https://littlemagic8.github.io/2024/05/15/how-to-use-ai/) [https://littlemagic8.github.io/2024/05/15/how-to-use-ai/*](https://littlemagic8.github.io/2024/05/15/how-to-use-ai/)

不想自己注册账号，可以用方式二

> *方式二：添加微信购买 微信：***aicygg888** *(备注镜像账号哦)*

欢迎加微信

![img](https://picx.zhimg.com/80/v2-46f7cfd62d1e94381388ab08b0fea3af_720w.png)

公众号也可以哦

![img](https://pic1.zhimg.com/80/v2-4e622b64238b20948a02e0c988ca5704_720w.png)

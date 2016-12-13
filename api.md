# API

配网 接口 回调函数

配置参数接口

OTA 接口


## external function

```
ej_ret ej_init_handle(ej_handler *handle);
```

```
ej_set_config
```


```
ej_ret ej_detroy_handle(ej_handler *handle);
```

```
ej_ret ej_set_channel(uint8_t *mac);
```

```
ej_ret ej_set_connect_callback(ej_callback lost_connect_callback, ej_callback restore_connect_callback);
```

```
ej_ret ej_set_thread_priority(int priority);
```

```
ej_ret ej_set_thread_stacksize(ej_handler *handle, int size);
```

```
ej_ret ej_connect(ej_handler *handler);
```

```
ej_ret ej_disconnect(ej_handler *handler);
```

```
//ej_ret ej_snd_proprity_msg(uint8_t *payload);
```

//
ej_ret ej_subscribe(uint8_t *topic, ej_callback func);

//
ej_set_network(int status)


set_sdk_log_level()

ej_printf(modue, ...);

// 

## internal function

```
timer_init
```

```
time_is_expired
```

```
time_countdown
```

```
time_left
```

```
network_init
```

```
network_connect
```

```
network_disconnect
```

```
network_write
```

```
network_read
```

```
network_udp_create
```

```
network_udp_bind
```

```
network_udp_write
```

```
network_udp_read
```

```
network_udp_close
```

```
mutex_init
```

```
mutex_lock
```

```
mutex_unlock
```

```
mutex_deinit
```

```
semaphore_int
```

```
semaphore_deinit
```

```
semaphore_wait
```

```
semaphore_post
```

```
thread_create(thread *th, init priority, const char *name, void (*founc)(void *), int stack_size, void *arg)
```

```
thread_join(thread *th, int)
```

```
thread_destroy(thread *th)
```

```
sleep(int ms);
```

```
plat_malloc(int size)
```

```
plat_free(void *mem); 
```

```
uart_open(UART_ID uart_id, uint32_t baudrate)
```

```
uart_close(UART_ID uart_id);
```

```
int16_t uart_read(const uint8_t *buf, uint32_t len);
```

```
int16_t uart_write(uint8_t *buf, uint32_t len);
```

```
printf
```

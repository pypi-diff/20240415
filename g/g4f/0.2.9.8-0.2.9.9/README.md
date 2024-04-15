# Comparing `tmp/g4f-0.2.9.8.tar.gz` & `tmp/g4f-0.2.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g4f-0.2.9.8.tar", last modified: Fri Apr 12 20:49:12 2024, max compression
+gzip compressed data, was "g4f-0.2.9.9.tar", last modified: Mon Apr 15 20:20:40 2024, max compression
```

## Comparing `g4f-0.2.9.8.tar` & `g4f-0.2.9.9.tar`

### file list

```diff
@@ -1,240 +1,240 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:12.280326 g4f-0.2.9.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-12 20:49:08.000000 g4f-0.2.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-12 20:49:08.000000 g4f-0.2.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    49179 2024-04-12 20:49:12.280326 g4f-0.2.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    45983 2024-04-12 20:49:08.000000 g4f-0.2.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:12.240326 g4f-0.2.9.8/g4f/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:12.248326 g4f-0.2.9.8/g4f/Provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/Aichatos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/Aura.py
--rw-r--r--   0 runner    (1001) docker     (127)    20942 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/Bing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/BingCreateImages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/Blackbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/ChatForAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/Chatgpt4Online.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/ChatgptAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/ChatgptFree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/ChatgptNext.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/ChatgptX.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/Cnote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/DeepInfra.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/DeepInfraImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/DuckDuckGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/Feedough.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/FlowGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/FreeChatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/FreeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/GeminiPro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/GeminiProChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/GigaChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/GptTalkRu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/HuggingChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/HuggingFace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/Koala.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/Liaobots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/Llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/Local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/PerplexityLabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/Pi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/ReplicateImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/WhiteRabbitNeo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/You.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/base_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:12.248326 g4f-0.2.9.8/g4f/Provider/bing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/bing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/bing/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/bing/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/bing/upload_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:12.256326 g4f-0.2.9.8/g4f/Provider/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/Acytoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/AiAsk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/AiChatOnline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/AiService.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/Aibn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/Aichat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/Ails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/Aivvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/Berlin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/ChatAnywhere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/ChatgptDuo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/CodeLinkAva.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/Cromicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/DfeHub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/EasyChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/Equing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/FakeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/FastGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/Forefront.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/GPTalk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/GeekGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/GetGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/H2o.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/Hashnode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/Lockchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/Myshell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/NoowAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/Opchatgpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/OpenAssistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/V50.py
--rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/Vitalentum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/VoiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/Wewordle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/Wuguokai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/Ylokh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/Yqcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/deprecated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:12.256326 g4f-0.2.9.8/g4f/Provider/gigachat_crt/
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:12.256326 g4f-0.2.9.8/g4f/Provider/needs_auth/
--rw-r--r--   0 runner    (1001) docker     (127)     8802 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/needs_auth/Gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/needs_auth/Groq.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/needs_auth/OpenRouter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/needs_auth/Openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    31632 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/needs_auth/OpenaiChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/needs_auth/Poe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/needs_auth/Raycast.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/needs_auth/Theb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/needs_auth/ThebApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/needs_auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:12.260326 g4f-0.2.9.8/g4f/Provider/not_working/
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/not_working/AItianhu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/not_working/Bestim.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/not_working/ChatBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/not_working/ChatgptDemo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/not_working/ChatgptDemoAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/not_working/ChatgptLogin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/not_working/Chatxyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/not_working/Gpt6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/not_working/GptChatly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/not_working/GptForLove.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/not_working/GptGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/not_working/GptGod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/not_working/OnlineGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/not_working/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:12.260326 g4f-0.2.9.8/g4f/Provider/npm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:12.260326 g4f-0.2.9.8/g4f/Provider/npm/node_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/npm/node_modules/.package-lock.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:12.260326 g4f-0.2.9.8/g4f/Provider/npm/node_modules/crypto-js/
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/npm/node_modules/crypto-js/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/npm/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/npm/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:12.260326 g4f-0.2.9.8/g4f/Provider/openai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/openai/crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/openai/har_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:12.264326 g4f-0.2.9.8/g4f/Provider/selenium/
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/selenium/AItianhuSpace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/selenium/Bard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/selenium/MyShell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/selenium/PerplexityAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/selenium/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/selenium/TalkAi.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/selenium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:12.264326 g4f-0.2.9.8/g4f/Provider/unfinished/
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/unfinished/AiChatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/unfinished/ChatAiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/unfinished/Komo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/unfinished/MikuChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/unfinished/Replicate.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/unfinished/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:12.264326 g4f-0.2.9.8/g4f/Provider/you/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/you/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/Provider/you/har_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:12.264326 g4f-0.2.9.8/g4f/api/
--rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/api/_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/api/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/api/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:12.264326 g4f-0.2.9.8/g4f/client/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7531 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/client/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/client/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/client/image_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/client/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/client/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:12.268326 g4f-0.2.9.8/g4f/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:12.268326 g4f-0.2.9.8/g4f/gui/client/
--rw-r--r--   0 runner    (1001) docker     (127)    12555 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/gui/client/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:12.236326 g4f-0.2.9.8/g4f/gui/client/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:12.268326 g4f-0.2.9.8/g4f/gui/client/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    22498 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/gui/client/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:12.268326 g4f-0.2.9.8/g4f/gui/client/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/gui/client/static/img/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/gui/client/static/img/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/gui/client/static/img/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/gui/client/static/img/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/gui/client/static/img/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/gui/client/static/img/gpt.png
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/gui/client/static/img/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/gui/client/static/img/user.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:12.268326 g4f-0.2.9.8/g4f/gui/client/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    45880 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/gui/client/static/js/chat.v1.js
--rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/gui/client/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/gui/client/static/js/highlightjs-copy.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/gui/client/static/js/icons.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:12.272326 g4f-0.2.9.8/g4f/gui/client/static/js/text_to_speech/
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/gui/client/static/js/text_to_speech/630.index.js
--rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/gui/client/static/js/text_to_speech/900.index.js
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/gui/client/static/js/text_to_speech/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/gui/gui_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/gui/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:12.272326 g4f-0.2.9.8/g4f/gui/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/gui/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/gui/server/android_gallery.py
--rw-r--r--   0 runner    (1001) docker     (127)     6365 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/gui/server/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/gui/server/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/gui/server/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/gui/server/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/gui/server/internet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/gui/server/js_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/gui/server/website.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/gui/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:12.272326 g4f-0.2.9.8/g4f/local/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:12.272326 g4f-0.2.9.8/g4f/locals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/locals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/locals/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/locals/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:12.276326 g4f-0.2.9.8/g4f/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9438 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/providers/base_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/providers/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/providers/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/providers/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/providers/retry_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/providers/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:12.276326 g4f-0.2.9.8/g4f/requests/
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/requests/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/requests/curl_cffi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/requests/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/requests/raise_for_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-04-12 20:49:08.000000 g4f-0.2.9.8/g4f/webdriver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:12.276326 g4f-0.2.9.8/g4f.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    49179 2024-04-12 20:49:12.000000 g4f-0.2.9.8/g4f.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-12 20:49:12.000000 g4f-0.2.9.8/g4f.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 20:49:12.000000 g4f-0.2.9.8/g4f.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-12 20:49:12.000000 g4f-0.2.9.8/g4f.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-12 20:49:12.000000 g4f-0.2.9.8/g4f.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-12 20:49:12.000000 g4f-0.2.9.8/g4f.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 20:49:12.280326 g4f-0.2.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-12 20:49:08.000000 g4f-0.2.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.024993 g4f-0.2.9.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-15 20:20:36.000000 g4f-0.2.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-15 20:20:36.000000 g4f-0.2.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    49881 2024-04-15 20:20:40.024993 g4f-0.2.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    46685 2024-04-15 20:20:36.000000 g4f-0.2.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:39.988992 g4f-0.2.9.9/g4f/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:39.996992 g4f-0.2.9.9/g4f/Provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/Aichatos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/Aura.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20942 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/Bing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/BingCreateImages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/Blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/ChatForAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/Chatgpt4Online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/ChatgptAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/ChatgptFree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/ChatgptNext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/ChatgptX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/Cnote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/DeepInfra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/DeepInfraImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/DuckDuckGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/Feedough.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/FlowGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/FreeChatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/FreeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/GeminiPro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/GeminiProChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/GigaChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/GptTalkRu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/HuggingChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/HuggingFace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/Koala.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/Liaobots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/Llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/Local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/PerplexityLabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/Pi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/ReplicateImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/WhiteRabbitNeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/You.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/base_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:39.996992 g4f-0.2.9.9/g4f/Provider/bing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/bing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/bing/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/bing/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/bing/upload_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.004992 g4f-0.2.9.9/g4f/Provider/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Acytoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/AiAsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/AiChatOnline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/AiService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Aibn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Aichat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Ails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Aivvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Berlin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/ChatAnywhere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/ChatgptDuo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/CodeLinkAva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Cromicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/DfeHub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/EasyChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Equing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/FakeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/FastGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Forefront.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/GPTalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/GeekGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/GetGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/H2o.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Hashnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Lockchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Myshell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/NoowAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Opchatgpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/OpenAssistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/V50.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Vitalentum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/VoiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Wewordle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Wuguokai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Ylokh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/Yqcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/deprecated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.004992 g4f-0.2.9.9/g4f/Provider/gigachat_crt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.004992 g4f-0.2.9.9/g4f/Provider/needs_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     8802 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/needs_auth/Gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/needs_auth/Groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/needs_auth/OpenRouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/needs_auth/Openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31953 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/needs_auth/OpenaiChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/needs_auth/Poe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/needs_auth/Raycast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/needs_auth/Theb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/needs_auth/ThebApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/needs_auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.008993 g4f-0.2.9.9/g4f/Provider/not_working/
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/not_working/AItianhu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/not_working/Bestim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/not_working/ChatBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/not_working/ChatgptDemo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/not_working/ChatgptDemoAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/not_working/ChatgptLogin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/not_working/Chatxyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/not_working/Gpt6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/not_working/GptChatly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/not_working/GptForLove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/not_working/GptGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/not_working/GptGod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/not_working/OnlineGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/not_working/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.008993 g4f-0.2.9.9/g4f/Provider/npm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.008993 g4f-0.2.9.9/g4f/Provider/npm/node_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/npm/node_modules/.package-lock.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.008993 g4f-0.2.9.9/g4f/Provider/npm/node_modules/crypto-js/
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/npm/node_modules/crypto-js/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/npm/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/npm/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.008993 g4f-0.2.9.9/g4f/Provider/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/openai/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/openai/har_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.012992 g4f-0.2.9.9/g4f/Provider/selenium/
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/selenium/AItianhuSpace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/selenium/Bard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/selenium/MyShell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/selenium/PerplexityAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/selenium/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/selenium/TalkAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/selenium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.012992 g4f-0.2.9.9/g4f/Provider/unfinished/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/unfinished/AiChatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/unfinished/ChatAiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/unfinished/Komo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/unfinished/MikuChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/unfinished/Replicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/unfinished/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.012992 g4f-0.2.9.9/g4f/Provider/you/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/you/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/Provider/you/har_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.012992 g4f-0.2.9.9/g4f/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/api/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/api/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/api/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.012992 g4f-0.2.9.9/g4f/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/client/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/client/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/client/image_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/client/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/client/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.012992 g4f-0.2.9.9/g4f/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.012992 g4f-0.2.9.9/g4f/gui/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    12555 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:39.984992 g4f-0.2.9.9/g4f/gui/client/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.016992 g4f-0.2.9.9/g4f/gui/client/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    22498 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.016992 g4f-0.2.9.9/g4f/gui/client/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/img/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/img/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/img/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/img/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/img/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/img/gpt.png
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/img/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/img/user.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.016992 g4f-0.2.9.9/g4f/gui/client/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    45661 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/js/chat.v1.js
+-rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/js/highlightjs-copy.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/js/icons.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.016992 g4f-0.2.9.9/g4f/gui/client/static/js/text_to_speech/
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/js/text_to_speech/630.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/js/text_to_speech/900.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/client/static/js/text_to_speech/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/gui_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.020993 g4f-0.2.9.9/g4f/gui/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/server/android_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6365 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/server/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/server/internet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/server/js_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/server/website.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/gui/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.020993 g4f-0.2.9.9/g4f/local/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.020993 g4f-0.2.9.9/g4f/locals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/locals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/locals/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/locals/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.020993 g4f-0.2.9.9/g4f/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9438 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/providers/base_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/providers/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/providers/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/providers/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8735 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/providers/retry_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/providers/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.020993 g4f-0.2.9.9/g4f/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/requests/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/requests/curl_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/requests/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/requests/raise_for_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-04-15 20:20:36.000000 g4f-0.2.9.9/g4f/webdriver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:20:40.020993 g4f-0.2.9.9/g4f.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    49881 2024-04-15 20:20:39.000000 g4f-0.2.9.9/g4f.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-15 20:20:39.000000 g4f-0.2.9.9/g4f.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:20:39.000000 g4f-0.2.9.9/g4f.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 20:20:39.000000 g4f-0.2.9.9/g4f.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-15 20:20:39.000000 g4f-0.2.9.9/g4f.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-15 20:20:39.000000 g4f-0.2.9.9/g4f.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 20:20:40.024993 g4f-0.2.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-15 20:20:36.000000 g4f-0.2.9.9/setup.py
```

### Comparing `g4f-0.2.9.8/LICENSE` & `g4f-0.2.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/PKG-INFO` & `g4f-0.2.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.2.9.8
+Version: 0.2.9.9
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
@@ -355,14 +355,24 @@
 | [chatgpt.ai](https://chatgpt.ai) | `g4f.Provider.ChatgptAi` | ❌ | ✔️ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
 | [liaobots.site](https://liaobots.site) | `g4f.Provider.Liaobots` | ✔️ | ✔️ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
 | [chat.openai.com](https://chat.openai.com) | `g4f.Provider.OpenaiChat` | ✔️ | ❌ | ✔️ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | ✔️ |
 | [raycast.com](https://raycast.com) | `g4f.Provider.Raycast` | ✔️ | ✔️ | ✔️ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | ✔️ |
 | [beta.theb.ai](https://beta.theb.ai) | `g4f.Provider.Theb` | ✔️ | ✔️ | ✔️ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | ❌ |
 | [you.com](https://you.com) | `g4f.Provider.You` | ✔️ | ✔️ | ✔️ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | ❌ |
 
+## Best OpenSource Models
+While we wait for gpt-5, here is a list of new models that are at least better than gpt-3.5-turbo. **Some are better than gpt-4**. Expect this list to grow.
+
+| Website | Provider |  parameters | better than |
+| ------  | -------  |  ------ |  ------ | 
+| [mixtral-8x22b](https://huggingface.co/mistral-community/Mixtral-8x22B-v0.1) | `g4f.Provider.DeepInfra` | 176B / 44b active | gpt-3.5-turbo |
+| [dbrx-instruct](https://www.databricks.com/blog/introducing-dbrx-new-state-art-open-llm) | `g4f.Provider.DeepInfra` | 132B / 36B active| gpt-3.5-turbo |
+| [command-r+](https://txt.cohere.com/command-r-plus-microsoft-azure/) | `g4f.Provider.HuggingChat` | 104B | gpt-4-0613 |
+
+
 ### GPT-3.5
 
 | Website | Provider | GPT-3.5 | GPT-4 | Stream | Status | Auth |
 | ------  | -------  | ------- | ----- | ------ | ------ | ---- |
 | [chat3.aiyunos.top](https://chat3.aiyunos.top/) | `g4f.Provider.AItianhuSpace` | ✔️ | ❌ | ✔️ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | ❌ |
 | [chatforai.store](https://chatforai.store) | `g4f.Provider.ChatForAi` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
 | [chatgpt4online.org](https://chatgpt4online.org) | `g4f.Provider.Chatgpt4Online` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.2.9.8 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.2.9.9 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
@@ -193,15 +193,24 @@
 [chat.openai.com](https://chat.openai.com) | `g4f.Provider.OpenaiChat` | âï¸
 | â | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | âï¸
 | | [raycast.com](https://raycast.com) | `g4f.Provider.Raycast` | âï¸ |
 âï¸ | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) |
 âï¸ | | [beta.theb.ai](https://beta.theb.ai) | `g4f.Provider.Theb` | âï¸
 | âï¸ | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | â
 | | [you.com](https://you.com) | `g4f.Provider.You` | âï¸ | âï¸ | âï¸
-| ![Unknown](https://img.shields.io/badge/Unknown-grey) | â | ### GPT-3.5 |
+| ![Unknown](https://img.shields.io/badge/Unknown-grey) | â | ## Best
+OpenSource Models While we wait for gpt-5, here is a list of new models that
+are at least better than gpt-3.5-turbo. **Some are better than gpt-4**. Expect
+this list to grow. | Website | Provider | parameters | better than | | ------ |
+------- | ------ | ------ | | [mixtral-8x22b](https://huggingface.co/mistral-
+community/Mixtral-8x22B-v0.1) | `g4f.Provider.DeepInfra` | 176B / 44b active |
+gpt-3.5-turbo | | [dbrx-instruct](https://www.databricks.com/blog/introducing-
+dbrx-new-state-art-open-llm) | `g4f.Provider.DeepInfra` | 132B / 36B active|
+gpt-3.5-turbo | | [command-r+](https://txt.cohere.com/command-r-plus-microsoft-
+azure/) | `g4f.Provider.HuggingChat` | 104B | gpt-4-0613 | ### GPT-3.5 |
 Website | Provider | GPT-3.5 | GPT-4 | Stream | Status | Auth | | ------ | ----
 --- | ------- | ----- | ------ | ------ | ---- | | [chat3.aiyunos.top](https://
 chat3.aiyunos.top/) | `g4f.Provider.AItianhuSpace` | âï¸ | â | âï¸ | !
 [Unknown](https://img.shields.io/badge/Unknown-grey) | â | |
 [chatforai.store](https://chatforai.store) | `g4f.Provider.ChatForAi` | âï¸
 | â | âï¸ | ![Active](https://img.shields.io/badge/Active-brightgreen) |
 â | | [chatgpt4online.org](https://chatgpt4online.org) |
```

### Comparing `g4f-0.2.9.8/README.md` & `g4f-0.2.9.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -277,14 +277,24 @@
 | [chatgpt.ai](https://chatgpt.ai) | `g4f.Provider.ChatgptAi` | ❌ | ✔️ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
 | [liaobots.site](https://liaobots.site) | `g4f.Provider.Liaobots` | ✔️ | ✔️ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
 | [chat.openai.com](https://chat.openai.com) | `g4f.Provider.OpenaiChat` | ✔️ | ❌ | ✔️ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | ✔️ |
 | [raycast.com](https://raycast.com) | `g4f.Provider.Raycast` | ✔️ | ✔️ | ✔️ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | ✔️ |
 | [beta.theb.ai](https://beta.theb.ai) | `g4f.Provider.Theb` | ✔️ | ✔️ | ✔️ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | ❌ |
 | [you.com](https://you.com) | `g4f.Provider.You` | ✔️ | ✔️ | ✔️ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | ❌ |
 
+## Best OpenSource Models
+While we wait for gpt-5, here is a list of new models that are at least better than gpt-3.5-turbo. **Some are better than gpt-4**. Expect this list to grow.
+
+| Website | Provider |  parameters | better than |
+| ------  | -------  |  ------ |  ------ | 
+| [mixtral-8x22b](https://huggingface.co/mistral-community/Mixtral-8x22B-v0.1) | `g4f.Provider.DeepInfra` | 176B / 44b active | gpt-3.5-turbo |
+| [dbrx-instruct](https://www.databricks.com/blog/introducing-dbrx-new-state-art-open-llm) | `g4f.Provider.DeepInfra` | 132B / 36B active| gpt-3.5-turbo |
+| [command-r+](https://txt.cohere.com/command-r-plus-microsoft-azure/) | `g4f.Provider.HuggingChat` | 104B | gpt-4-0613 |
+
+
 ### GPT-3.5
 
 | Website | Provider | GPT-3.5 | GPT-4 | Stream | Status | Auth |
 | ------  | -------  | ------- | ----- | ------ | ------ | ---- |
 | [chat3.aiyunos.top](https://chat3.aiyunos.top/) | `g4f.Provider.AItianhuSpace` | ✔️ | ❌ | ✔️ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | ❌ |
 | [chatforai.store](https://chatforai.store) | `g4f.Provider.ChatForAi` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
 | [chatgpt4online.org](https://chatgpt4online.org) | `g4f.Provider.Chatgpt4Online` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
```

#### html2text {}

```diff
@@ -151,15 +151,24 @@
 [chat.openai.com](https://chat.openai.com) | `g4f.Provider.OpenaiChat` | âï¸
 | â | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | âï¸
 | | [raycast.com](https://raycast.com) | `g4f.Provider.Raycast` | âï¸ |
 âï¸ | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) |
 âï¸ | | [beta.theb.ai](https://beta.theb.ai) | `g4f.Provider.Theb` | âï¸
 | âï¸ | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | â
 | | [you.com](https://you.com) | `g4f.Provider.You` | âï¸ | âï¸ | âï¸
-| ![Unknown](https://img.shields.io/badge/Unknown-grey) | â | ### GPT-3.5 |
+| ![Unknown](https://img.shields.io/badge/Unknown-grey) | â | ## Best
+OpenSource Models While we wait for gpt-5, here is a list of new models that
+are at least better than gpt-3.5-turbo. **Some are better than gpt-4**. Expect
+this list to grow. | Website | Provider | parameters | better than | | ------ |
+------- | ------ | ------ | | [mixtral-8x22b](https://huggingface.co/mistral-
+community/Mixtral-8x22B-v0.1) | `g4f.Provider.DeepInfra` | 176B / 44b active |
+gpt-3.5-turbo | | [dbrx-instruct](https://www.databricks.com/blog/introducing-
+dbrx-new-state-art-open-llm) | `g4f.Provider.DeepInfra` | 132B / 36B active|
+gpt-3.5-turbo | | [command-r+](https://txt.cohere.com/command-r-plus-microsoft-
+azure/) | `g4f.Provider.HuggingChat` | 104B | gpt-4-0613 | ### GPT-3.5 |
 Website | Provider | GPT-3.5 | GPT-4 | Stream | Status | Auth | | ------ | ----
 --- | ------- | ----- | ------ | ------ | ---- | | [chat3.aiyunos.top](https://
 chat3.aiyunos.top/) | `g4f.Provider.AItianhuSpace` | âï¸ | â | âï¸ | !
 [Unknown](https://img.shields.io/badge/Unknown-grey) | â | |
 [chatforai.store](https://chatforai.store) | `g4f.Provider.ChatForAi` | âï¸
 | â | âï¸ | ![Active](https://img.shields.io/badge/Active-brightgreen) |
 â | | [chatgpt4online.org](https://chatgpt4online.org) |
```

### Comparing `g4f-0.2.9.8/g4f/Provider/Aichatos.py` & `g4f-0.2.9.9/g4f/Provider/Aichatos.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/Aura.py` & `g4f-0.2.9.9/g4f/Provider/Aura.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/Bing.py` & `g4f-0.2.9.9/g4f/Provider/Bing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/BingCreateImages.py` & `g4f-0.2.9.9/g4f/Provider/BingCreateImages.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/Blackbox.py` & `g4f-0.2.9.9/g4f/Provider/Blackbox.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/ChatForAi.py` & `g4f-0.2.9.9/g4f/Provider/ChatForAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/Chatgpt4Online.py` & `g4f-0.2.9.9/g4f/Provider/Chatgpt4Online.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/ChatgptAi.py` & `g4f-0.2.9.9/g4f/Provider/ChatgptAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/ChatgptFree.py` & `g4f-0.2.9.9/g4f/Provider/ChatgptFree.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/ChatgptNext.py` & `g4f-0.2.9.9/g4f/Provider/ChatgptNext.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/ChatgptX.py` & `g4f-0.2.9.9/g4f/Provider/ChatgptX.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/Cnote.py` & `g4f-0.2.9.9/g4f/Provider/Cnote.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/DeepInfra.py` & `g4f-0.2.9.9/g4f/Provider/DeepInfra.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class DeepInfra(Openai):
     label = "DeepInfra"
     url = "https://deepinfra.com"
     working = True
     needs_auth = False
     supports_stream = True
     supports_message_history = True
-    default_model = 'meta-llama/Llama-2-70b-chat-hf'
+    default_model = 'HuggingFaceH4/zephyr-orpo-141b-A35b-v0.1'
 
     @classmethod
     def get_models(cls):
         if not cls.models:
             url = 'https://api.deepinfra.com/models/featured'
             models = requests.get(url).json()
             cls.models = [model['model_name'] for model in models if model["type"] == "text-generation"]
@@ -28,14 +28,22 @@
         messages: Messages,
         stream: bool,
         api_base: str = "https://api.deepinfra.com/v1/openai",
         temperature: float = 0.7,
         max_tokens: int = 1028,
         **kwargs
     ) -> AsyncResult:
+        
+        if not '/' in model:
+            models = {
+                'mixtral-8x22b': 'HuggingFaceH4/zephyr-orpo-141b-A35b-v0.1',
+                'dbrx-instruct': 'databricks/dbrx-instruct',
+            }
+            model = models.get(model, model)
+        
         headers = {
             'Accept-Encoding': 'gzip, deflate, br',
             'Accept-Language': 'en-US',
             'Connection': 'keep-alive',
             'Origin': 'https://deepinfra.com',
             'Referer': 'https://deepinfra.com/',
             'Sec-Fetch-Dest': 'empty',
```

### Comparing `g4f-0.2.9.8/g4f/Provider/DeepInfraImage.py` & `g4f-0.2.9.9/g4f/Provider/DeepInfraImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/DuckDuckGo.py` & `g4f-0.2.9.9/g4f/Provider/DuckDuckGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/Feedough.py` & `g4f-0.2.9.9/g4f/Provider/Feedough.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/FlowGpt.py` & `g4f-0.2.9.9/g4f/Provider/FlowGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/FreeChatgpt.py` & `g4f-0.2.9.9/g4f/Provider/FreeChatgpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/FreeGpt.py` & `g4f-0.2.9.9/g4f/Provider/FreeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/GeminiPro.py` & `g4f-0.2.9.9/g4f/Provider/GeminiPro.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/GeminiProChat.py` & `g4f-0.2.9.9/g4f/Provider/GeminiProChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/GigaChat.py` & `g4f-0.2.9.9/g4f/Provider/GigaChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/GptTalkRu.py` & `g4f-0.2.9.9/g4f/Provider/GptTalkRu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/HuggingChat.py` & `g4f-0.2.9.9/g4f/Provider/HuggingChat.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,21 +10,20 @@
 from .helper import format_prompt, get_connector
 
 class HuggingChat(AsyncGeneratorProvider, ProviderModelMixin):
     url = "https://huggingface.co/chat"
     working = True
     default_model = "mistralai/Mixtral-8x7B-Instruct-v0.1"
     models = [
-        "mistralai/Mixtral-8x7B-Instruct-v0.1",
-        "google/gemma-7b-it",
-        "meta-llama/Llama-2-70b-chat-hf",
-        "NousResearch/Nous-Hermes-2-Mixtral-8x7B-DPO",
-        "codellama/CodeLlama-34b-Instruct-hf",
-        "mistralai/Mistral-7B-Instruct-v0.2",
-        "openchat/openchat-3.5-0106",
+        "HuggingFaceH4/zephyr-orpo-141b-A35b-v0.1",
+        'CohereForAI/c4ai-command-r-plus',
+        'mistralai/Mixtral-8x7B-Instruct-v0.1',
+        'google/gemma-1.1-7b-it',
+        'NousResearch/Nous-Hermes-2-Mixtral-8x7B-DPO',
+        'mistralai/Mistral-7B-Instruct-v0.2'
     ]
     model_aliases = {
         "openchat/openchat_3.5": "openchat/openchat-3.5-0106",
     }
 
     @classmethod
     def get_models(cls):
@@ -44,14 +43,15 @@
         proxy: str = None,
         connector: BaseConnector = None,
         web_search: bool = False,
         cookies: dict = None,
         **kwargs
     ) -> AsyncResult:
         options = {"model": cls.get_model(model)}
+
         system_prompt = "\n".join([message["content"] for message in messages if message["role"] == "system"])
         if system_prompt:
             options["preprompt"] = system_prompt
             messages = [message for message in messages if message["role"] != "system"]
         headers = {
             'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36',
         }
```

### Comparing `g4f-0.2.9.8/g4f/Provider/HuggingFace.py` & `g4f-0.2.9.9/g4f/Provider/HuggingFace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/Koala.py` & `g4f-0.2.9.9/g4f/Provider/Koala.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/Liaobots.py` & `g4f-0.2.9.9/g4f/Provider/Liaobots.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/Llama2.py` & `g4f-0.2.9.9/g4f/Provider/Llama2.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/Local.py` & `g4f-0.2.9.9/g4f/Provider/Local.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/PerplexityLabs.py` & `g4f-0.2.9.9/g4f/Provider/PerplexityLabs.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,21 +15,22 @@
     url = "https://labs.perplexity.ai"    
     working = True
     default_model = "mixtral-8x7b-instruct"
     models = [
         "sonar-small-online", "sonar-medium-online", "sonar-small-chat", "sonar-medium-chat", "mistral-7b-instruct", 
         "codellama-70b-instruct", "llava-v1.5-7b-wrapper", "llava-v1.6-34b", "mixtral-8x7b-instruct",
         "gemma-2b-it", "gemma-7b-it"
-        "mistral-medium", "related"
+        "mistral-medium", "related", "dbrx-instruct"
     ]
     model_aliases = {
         "mistralai/Mistral-7B-Instruct-v0.1": "mistral-7b-instruct", 
         "mistralai/Mixtral-8x7B-Instruct-v0.1": "mixtral-8x7b-instruct",
         "codellama/CodeLlama-70b-Instruct-hf": "codellama-70b-instruct",
-        "llava-v1.5-7b": "llava-v1.5-7b-wrapper"
+        "llava-v1.5-7b": "llava-v1.5-7b-wrapper",
+        'databricks/dbrx-instruct': "dbrx-instruct"
     }
 
     @classmethod
     async def create_async_generator(
         cls,
         model: str,
         messages: Messages,
```

### Comparing `g4f-0.2.9.8/g4f/Provider/Pi.py` & `g4f-0.2.9.9/g4f/Provider/Pi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/ReplicateImage.py` & `g4f-0.2.9.9/g4f/Provider/ReplicateImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/Vercel.py` & `g4f-0.2.9.9/g4f/Provider/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/WhiteRabbitNeo.py` & `g4f-0.2.9.9/g4f/Provider/WhiteRabbitNeo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/You.py` & `g4f-0.2.9.9/g4f/Provider/You.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
             model = cls.get_model(model)
         async with StreamSession(
             proxies={"all": proxy},
             impersonate="chrome",
             timeout=(30, timeout)
         ) as session:
             cookies = await cls.get_cookies(session) if chat_mode != "default" else None
+            
             upload = json.dumps([await cls.upload_file(session, cookies, to_bytes(image), image_name)]) if image else ""
             headers = {
                 "Accept": "text/event-stream",
                 "Referer": f"{cls.url}/search?fromSearchBar=true&tbm=youchat",
             }
             data = {
                 "userFiles": upload,
@@ -127,14 +128,15 @@
             result = await response.json()
         result["user_filename"] = filename
         result["size"] = len(file)
         return result
 
     @classmethod
     async def get_cookies(cls, client: StreamSession) -> Cookies:
+
         if not cls._cookies or cls._cookies_used >= 5:
             cls._cookies = await cls.create_cookies(client)
             cls._cookies_used = 0
         cls._cookies_used += 1
         return cls._cookies        
 
     @classmethod
@@ -147,16 +149,16 @@
             "stytch_user_id":f"user-live-{uuid.uuid4()}",
             "stytch_session_id":f"session-live-{uuid.uuid4()}",
             "app":{"identifier":"you.com"},
             "sdk":{"identifier":"Stytch.js Javascript SDK","version":"3.3.0"
         }}).encode()).decode()
 
     def get_auth() -> str:
-        auth_uuid = "507a52ad-7e69-496b-aee0-1c9863c7c8"
-        auth_token = f"public-token-live-{auth_uuid}bb:public-token-live-{auth_uuid}19"
+        auth_uuid = "507a52ad-7e69-496b-aee0-1c9863c7c819"
+        auth_token = f"public-token-live-{auth_uuid}:public-token-live-{auth_uuid}"
         auth = base64.standard_b64encode(auth_token.encode()).decode()
         return f"Basic {auth}"
 
     @classmethod
     async def create_cookies(cls, client: StreamSession) -> Cookies:
         user_uuid = str(uuid.uuid4())
         async with client.post(
@@ -168,19 +170,19 @@
                 "Origin": "https://you.com",
                 "Referer": "https://you.com/"
             },
             json={
                 "dfp_telemetry_id": await get_dfp_telemetry_id(),
                 "email": f"{user_uuid}@gmail.com",
                 "password": f"{user_uuid}#{user_uuid}",
-                "dfp_telemetry_id": f"{uuid.uuid4()}",
                 "session_duration_minutes": 129600
             }
         ) as response:
             await raise_for_status(response)
             session = (await response.json())["data"]
+
         return {
             "stytch_session": session["session_token"],
             'stytch_session_jwt': session["session_jwt"],
             'ydc_stytch_session': session["session_token"],
             'ydc_stytch_session_jwt': session["session_jwt"],
         }
```

### Comparing `g4f-0.2.9.8/g4f/Provider/__init__.py` & `g4f-0.2.9.9/g4f/Provider/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/bing/conversation.py` & `g4f-0.2.9.9/g4f/Provider/bing/conversation.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/bing/create_images.py` & `g4f-0.2.9.9/g4f/Provider/bing/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/bing/upload_image.py` & `g4f-0.2.9.9/g4f/Provider/bing/upload_image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/Acytoo.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/Acytoo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/AiAsk.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/AiAsk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/AiChatOnline.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/AiChatOnline.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/AiService.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/AiService.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/Aibn.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/Aibn.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/Aichat.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/Aichat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/Ails.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/Ails.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/Aivvm.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/Aivvm.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/Berlin.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/Berlin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/ChatAnywhere.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/ChatAnywhere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/ChatgptDuo.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/ChatgptDuo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/CodeLinkAva.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/CodeLinkAva.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/Cromicle.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/Cromicle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/DfeHub.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/DfeHub.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/EasyChat.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/EasyChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/Equing.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/Equing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/FakeGpt.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/FakeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/FastGpt.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/FastGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/Forefront.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/Forefront.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/GPTalk.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/GPTalk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/GeekGpt.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/GeekGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/GetGpt.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/GetGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/H2o.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/H2o.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/Hashnode.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/Hashnode.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/Lockchat.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/Lockchat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/Myshell.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/Myshell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/NoowAi.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/NoowAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/Opchatgpts.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/Opchatgpts.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/OpenAssistant.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/OpenAssistant.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/Phind.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/V50.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/V50.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/Vercel.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/Vitalentum.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/Vitalentum.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/VoiGpt.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/VoiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/Wewordle.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/Wewordle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/Wuguokai.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/Wuguokai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/Ylokh.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/Ylokh.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/Yqcloud.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/Yqcloud.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/deprecated/__init__.py` & `g4f-0.2.9.9/g4f/Provider/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt` & `g4f-0.2.9.9/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/needs_auth/Gemini.py` & `g4f-0.2.9.9/g4f/Provider/needs_auth/Gemini.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/needs_auth/Groq.py` & `g4f-0.2.9.9/g4f/Provider/needs_auth/Groq.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/needs_auth/OpenRouter.py` & `g4f-0.2.9.9/g4f/Provider/needs_auth/OpenRouter.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/needs_auth/Openai.py` & `g4f-0.2.9.9/g4f/Provider/needs_auth/Openai.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,15 @@
                 temperature=temperature,
                 max_tokens=max_tokens,
                 top_p=top_p,
                 stop=stop,
                 stream=stream,
                 **extra_data
             )
+            
             async with session.post(f"{api_base.rstrip('/')}/chat/completions", json=data) as response:
                 await raise_for_status(response)
                 if not stream:
                     data = await response.json()
                     choice = data["choices"][0]
                     if "content" in choice["message"]:
                         yield choice["message"]["content"].strip()
```

### Comparing `g4f-0.2.9.8/g4f/Provider/needs_auth/OpenaiChat.py` & `g4f-0.2.9.9/g4f/Provider/needs_auth/OpenaiChat.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     working = True
     supports_gpt_35_turbo = True
     supports_gpt_4 = True
     supports_message_history = True
     supports_system_message = True
     default_model = None
     models = ["gpt-3.5-turbo", "gpt-4", "gpt-4-gizmo"]
-    model_aliases = {"text-davinci-002-render-sha": "gpt-3.5-turbo", "": "gpt-3.5-turbo"}
+    model_aliases = {"text-davinci-002-render-sha": "gpt-3.5-turbo", "": "gpt-3.5-turbo", "gpt-4-turbo-preview": "gpt-4"}
     _api_key: str = None
     _headers: dict = None
     _cookies: Cookies = None
     _expires: int = None
 
     @classmethod
     async def create(
@@ -330,14 +330,15 @@
 
         Yields:
             AsyncResult: Asynchronous results from the generator.
 
         Raises:
             RuntimeError: If an error occurs during processing.
         """
+
         async with StreamSession(
             proxies={"all": proxy},
             impersonate="chrome",
             timeout=timeout
         ) as session:
             if cls._expires is not None and cls._expires < time.time():
                 cls._headers = cls._api_key = None
@@ -355,24 +356,27 @@
                         cls.default_model = cls.get_model(model)
                 except Exception as e:
                     api_key = cls._api_key = None
                     cls._create_request_args()
                     if debug.logging:
                         print("OpenaiChat: Load default_model failed")
                         print(f"{e.__class__.__name__}: {e}")
+                        
 
             arkose_token = None
             if cls.default_model is None:
                 try:
                     arkose_token, api_key, cookies = await getArkoseAndAccessToken(proxy)
                     cls._create_request_args(cookies)
                     cls._set_api_key(api_key)
                 except NoValidHarFileError:
                     ...
                 if cls._api_key is None:
+                    if debug.logging:
+                        print("Getting access token with nodriver.")
                     await cls.nodriver_access_token()
                 cls.default_model = cls.get_model(await cls.get_default_model(session, cls._headers))
 
             async with session.post(
                 f"{cls.url}/backend-anon/sentinel/chat-requirements" if not cls._api_key else
                 f"{cls.url}/backend-api/sentinel/chat-requirements",
                 json={"conversation_mode_kind": "primary_assistant"},
@@ -380,14 +384,17 @@
             ) as response:
                 cls._update_request_args(session)
                 await raise_for_status(response)
                 data = await response.json()
                 blob = data["arkose"]["dx"]
                 need_arkose = data["arkose"]["required"]
                 chat_token = data["token"]
+                
+                if debug.logging:
+                    print(f'Arkose: {need_arkose} Turnstile: {data["turnstile"]["required"]}')
 
             if need_arkose and arkose_token is None:
                 arkose_token, api_key, cookies = await getArkoseAndAccessToken(proxy)
                 cls._create_request_args(cookies)
                 cls._set_api_key(api_key)
                 if arkose_token is None:
                     raise MissingAuthError("No arkose token found in .har file")
@@ -578,14 +585,15 @@
         except ImportError:
             return
         try:
             from platformdirs import user_config_dir
             user_data_dir = user_config_dir("g4f-nodriver")
         except:
             user_data_dir = None
+        
         browser = await uc.start(user_data_dir=user_data_dir)
         page = await browser.get("https://chat.openai.com/")
         while await page.query_selector("#prompt-textarea") is None:
             await asyncio.sleep(1)
         api_key = await page.evaluate(
             "(async () => {"
             "let session = await fetch('/api/auth/session');"
@@ -777,8 +785,8 @@
             **await self.get_fields(),
             **kwargs
         )
 
     async def get_messages(self) -> list:
         messages = self._messages
         messages.append({"role": "assistant", "content": await self.message()})
-        return messages
+        return messages
```

### Comparing `g4f-0.2.9.8/g4f/Provider/needs_auth/Poe.py` & `g4f-0.2.9.9/g4f/Provider/needs_auth/Poe.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/needs_auth/Raycast.py` & `g4f-0.2.9.9/g4f/Provider/needs_auth/Raycast.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/needs_auth/Theb.py` & `g4f-0.2.9.9/g4f/Provider/needs_auth/Theb.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/needs_auth/ThebApi.py` & `g4f-0.2.9.9/g4f/Provider/needs_auth/ThebApi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/not_working/AItianhu.py` & `g4f-0.2.9.9/g4f/Provider/not_working/AItianhu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/not_working/Bestim.py` & `g4f-0.2.9.9/g4f/Provider/not_working/Bestim.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/not_working/ChatBase.py` & `g4f-0.2.9.9/g4f/Provider/not_working/ChatBase.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/not_working/ChatgptDemo.py` & `g4f-0.2.9.9/g4f/Provider/not_working/ChatgptDemo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/not_working/ChatgptDemoAi.py` & `g4f-0.2.9.9/g4f/Provider/not_working/ChatgptDemoAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/not_working/ChatgptLogin.py` & `g4f-0.2.9.9/g4f/Provider/not_working/ChatgptLogin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/not_working/Chatxyz.py` & `g4f-0.2.9.9/g4f/Provider/not_working/Chatxyz.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/not_working/Gpt6.py` & `g4f-0.2.9.9/g4f/Provider/not_working/Gpt6.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/not_working/GptChatly.py` & `g4f-0.2.9.9/g4f/Provider/not_working/GptChatly.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/not_working/GptForLove.py` & `g4f-0.2.9.9/g4f/Provider/not_working/GptForLove.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/not_working/GptGo.py` & `g4f-0.2.9.9/g4f/Provider/not_working/GptGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/not_working/GptGod.py` & `g4f-0.2.9.9/g4f/Provider/not_working/GptGod.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/not_working/OnlineGpt.py` & `g4f-0.2.9.9/g4f/Provider/not_working/OnlineGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/npm/node_modules/crypto-js/README.md` & `g4f-0.2.9.9/g4f/Provider/npm/node_modules/crypto-js/README.md`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js` & `g4f-0.2.9.9/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/npm/package-lock.json` & `g4f-0.2.9.9/g4f/Provider/npm/package-lock.json`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/openai/crypt.py` & `g4f-0.2.9.9/g4f/Provider/openai/crypt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/openai/har_file.py` & `g4f-0.2.9.9/g4f/Provider/openai/har_file.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/selenium/AItianhuSpace.py` & `g4f-0.2.9.9/g4f/Provider/selenium/AItianhuSpace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/selenium/Bard.py` & `g4f-0.2.9.9/g4f/Provider/selenium/Bard.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/selenium/MyShell.py` & `g4f-0.2.9.9/g4f/Provider/selenium/MyShell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/selenium/PerplexityAi.py` & `g4f-0.2.9.9/g4f/Provider/selenium/PerplexityAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/selenium/Phind.py` & `g4f-0.2.9.9/g4f/Provider/selenium/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/selenium/TalkAi.py` & `g4f-0.2.9.9/g4f/Provider/selenium/TalkAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/unfinished/AiChatting.py` & `g4f-0.2.9.9/g4f/Provider/unfinished/AiChatting.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/unfinished/ChatAiGpt.py` & `g4f-0.2.9.9/g4f/Provider/unfinished/ChatAiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/unfinished/Komo.py` & `g4f-0.2.9.9/g4f/Provider/unfinished/Komo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/unfinished/MikuChat.py` & `g4f-0.2.9.9/g4f/Provider/unfinished/MikuChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/Provider/unfinished/Replicate.py` & `g4f-0.2.9.9/g4f/Provider/unfinished/Replicate.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/__init__.py` & `g4f-0.2.9.9/g4f/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/api/__init__.py` & `g4f-0.2.9.9/g4f/api/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/api/_logging.py` & `g4f-0.2.9.9/g4f/api/_logging.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/cli.py` & `g4f-0.2.9.9/g4f/cli.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/client/async_client.py` & `g4f-0.2.9.9/g4f/client/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         stop = [stop] if isinstance(stop, str) else stop
         response = create_response(
             messages, model,
             provider, stream,
             proxy=self.client.get_proxy() if proxy is None else proxy,
             max_tokens=max_tokens,
             stop=stop,
-            api_key=self.client.api_key if api_key is None else api_key
+            api_key=self.client.api_key if api_key is None else api_key,
             **kwargs
         )
         response = iter_response(response, stream, response_format, max_tokens, stop)
         response = iter_append_model_and_provider(response)
         return response if stream else anext(response)
 
 class Chat():
@@ -203,8 +203,8 @@
                 image=image,
                 proxy=self.client.get_proxy(),
                 **kwargs
             )
             result = iter_image_response(response)
         if result is None:
             raise NoImageResponseError()
-        return result
+        return result
```

### Comparing `g4f-0.2.9.8/g4f/client/client.py` & `g4f-0.2.9.9/g4f/client/client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/client/helper.py` & `g4f-0.2.9.9/g4f/client/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/client/image_models.py` & `g4f-0.2.9.9/g4f/client/image_models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/client/service.py` & `g4f-0.2.9.9/g4f/client/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,17 +51,18 @@
         debug.version_check = False
         version.utils.check_version()
 
     if isinstance(provider, str):
         provider = convert_to_provider(provider)
 
     if isinstance(model, str):
+        
         if model in ModelUtils.convert:
             model = ModelUtils.convert[model]
-
+    
     if not provider:
         if isinstance(model, str):
             raise ModelNotFoundError(f'Model not found: {model}')
         provider = model.best_provider
 
     if not provider:
         raise ProviderNotFoundError(f'No provider found for model: {model}')
```

### Comparing `g4f-0.2.9.8/g4f/client/stubs.py` & `g4f-0.2.9.9/g4f/client/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/client/types.py` & `g4f-0.2.9.9/g4f/client/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/cookies.py` & `g4f-0.2.9.9/g4f/cookies.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/errors.py` & `g4f-0.2.9.9/g4f/errors.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/gui/__init__.py` & `g4f-0.2.9.9/g4f/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/gui/client/index.html` & `g4f-0.2.9.9/g4f/gui/client/index.html`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/gui/client/static/css/style.css` & `g4f-0.2.9.9/g4f/gui/client/static/css/style.css`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/gui/client/static/img/android-chrome-192x192.png` & `g4f-0.2.9.9/g4f/gui/client/static/img/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/gui/client/static/img/android-chrome-512x512.png` & `g4f-0.2.9.9/g4f/gui/client/static/img/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/gui/client/static/img/apple-touch-icon.png` & `g4f-0.2.9.9/g4f/gui/client/static/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/gui/client/static/img/favicon-32x32.png` & `g4f-0.2.9.9/g4f/gui/client/static/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/gui/client/static/img/gpt.png` & `g4f-0.2.9.9/g4f/gui/client/static/img/gpt.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/gui/client/static/img/user.png` & `g4f-0.2.9.9/g4f/gui/client/static/img/user.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/gui/client/static/js/chat.v1.js` & `g4f-0.2.9.9/g4f/gui/client/static/js/chat.v1.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1081,23 +1081,23 @@
     } else {
         text += versions["version"];
     }
     document.getElementById("version_text").innerHTML = text
 }
 setTimeout(load_version, 2000);
 
-for (const el of [imageInput, cameraInput]) {
+[imageInput, cameraInput].forEach((el) => {
     el.addEventListener('click', async () => {
         el.value = '';
         if (imageInput.dataset.src) {
             URL.revokeObjectURL(imageInput.dataset.src);
             delete imageInput.dataset.src
         }
     });
-}
+});
 
 fileInput.addEventListener('click', async (event) => {
     fileInput.value = '';
     delete fileInput.dataset.text;
 });
 
 fileInput.addEventListener('change', async (event) => {
@@ -1277,39 +1277,34 @@
     mircoIcon.classList.remove("fa-microphone-slash");
 
     const recognition = new SpeechRecognition();
     recognition.continuous = true;
     recognition.interimResults = true;
     recognition.maxAlternatives = 1;
 
-    function may_stop() {
-        if (microLabel.classList.contains("recognition")) {
-            recognition.stop();
-        }
-    }
-
     let startValue;
-    let timeoutHandle;
+    let shouldStop;
     let lastDebounceTranscript;
     recognition.onstart = function() {
         microLabel.classList.add("recognition");
         startValue = messageInput.value;
+        shouldStop = false;
         lastDebounceTranscript = "";
-        timeoutHandle = window.setTimeout(may_stop, 10000);
     };
     recognition.onend = function() {
-        microLabel.classList.remove("recognition");
-        messageInput.focus();
+        if (shouldStop) {
+            messageInput.focus();
+        } else {
+            recognition.start();
+        }
     };
     recognition.onresult = function(event) {
         if (!event.results) {
             return;
         }
-        window.clearTimeout(timeoutHandle);
-
         let result = event.results[event.resultIndex];
         let isFinal = result.isFinal && (result[0].confidence > 0);
         let transcript = result[0].transcript;
         if (isFinal) {
             if (transcript == lastDebounceTranscript) {
                 return;
             }
@@ -1319,22 +1314,21 @@
             messageInput.value = `${startValue ? startValue+"\n" : ""}${transcript.trim()}`;
             if (isFinal) {
                 startValue = messageInput.value;
             }
             messageInput.style.height = messageInput.scrollHeight + "px";
             messageInput.scrollTop = messageInput.scrollHeight;
         }
-
-        timeoutHandle = window.setTimeout(may_stop, transcript ? 10000 : 8000);
     };
 
     microLabel.addEventListener("click", () => {
         if (microLabel.classList.contains("recognition")) {
-            window.clearTimeout(timeoutHandle);
+            shouldStop = true;
             recognition.stop();
+            microLabel.classList.remove("recognition");
         } else {
             const lang = document.getElementById("recognition-language")?.value;
             recognition.lang = lang || navigator.language;
             recognition.start();
         }
     });
 }
```

### Comparing `g4f-0.2.9.8/g4f/gui/client/static/js/highlight.min.js` & `g4f-0.2.9.9/g4f/gui/client/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/gui/client/static/js/highlightjs-copy.min.js` & `g4f-0.2.9.9/g4f/gui/client/static/js/highlightjs-copy.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/gui/client/static/js/icons.js` & `g4f-0.2.9.9/g4f/gui/client/static/js/icons.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/gui/client/static/js/text_to_speech/630.index.js` & `g4f-0.2.9.9/g4f/gui/client/static/js/text_to_speech/630.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/gui/client/static/js/text_to_speech/900.index.js` & `g4f-0.2.9.9/g4f/gui/client/static/js/text_to_speech/900.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/gui/client/static/js/text_to_speech/index.js` & `g4f-0.2.9.9/g4f/gui/client/static/js/text_to_speech/index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/gui/server/android_gallery.py` & `g4f-0.2.9.9/g4f/gui/server/android_gallery.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/gui/server/api.py` & `g4f-0.2.9.9/g4f/gui/server/api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/gui/server/backend.py` & `g4f-0.2.9.9/g4f/gui/server/backend.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/gui/server/config.py` & `g4f-0.2.9.9/g4f/gui/server/config.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/gui/server/internet.py` & `g4f-0.2.9.9/g4f/gui/server/internet.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/gui/server/js_api.py` & `g4f-0.2.9.9/g4f/gui/server/js_api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/gui/server/website.py` & `g4f-0.2.9.9/g4f/gui/server/website.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/gui/webview.py` & `g4f-0.2.9.9/g4f/gui/webview.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/image.py` & `g4f-0.2.9.9/g4f/image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/local/__init__.py` & `g4f-0.2.9.9/g4f/local/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/locals/models.py` & `g4f-0.2.9.9/g4f/locals/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/locals/provider.py` & `g4f-0.2.9.9/g4f/locals/provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/models.py` & `g4f-0.2.9.9/g4f/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     name          = 'gpt-3.5-turbo',
     base_provider = 'openai',
     best_provider = RetryProvider([
         FreeGpt,
         You,
         ChatgptNext,
         Koala,
+        OpenaiChat,
     ])
 )
 
 gpt_4 = Model(
     name          = 'gpt-4',
     base_provider = 'openai',
     best_provider = RetryProvider([
@@ -157,19 +158,19 @@
 
 mistral_7b_v02 = Model(
     name          = "mistralai/Mistral-7B-Instruct-v0.2",
     base_provider = "huggingface",
     best_provider = DeepInfra
 )
 
-# mixtral_8x22b = Model(
-#     name          = "mistralai/Mixtral-8x22B-v0.1",
-#     base_provider = "huggingface",
-#     best_provider = DeepInfra
-# )
+mixtral_8x22b = Model(
+    name          = "HuggingFaceH4/zephyr-orpo-141b-A35b-v0.1",
+    base_provider = "huggingface",
+    best_provider = RetryProvider([HuggingChat, DeepInfra])
+)
 
 # Misc models
 dolphin_mixtral_8x7b = Model(
     name          = "cognitivecomputations/dolphin-2.6-mixtral-8x7b",
     base_provider = "huggingface",
     best_provider = DeepInfra
 )
@@ -261,14 +262,26 @@
 
 pi = Model(
     name = 'pi',
     base_provider = 'inflection',
     best_provider = Pi
 )
 
+dbrx_instruct = Model(
+    name = 'databricks/dbrx-instruct',
+    base_provider = 'mistral',
+    best_provider = RetryProvider([DeepInfra, PerplexityLabs])
+)
+
+command_r_plus = Model(
+    name = 'CohereForAI/c4ai-command-r-plus',
+    base_provider = 'mistral',
+    best_provider = HuggingChat
+)
+
 class ModelUtils:
     """
     Utility class for mapping string identifiers to Model instances.
 
     Attributes:
         convert (dict[str, Model]): Dictionary mapping model string identifiers to Model instances.
     """
@@ -295,25 +308,34 @@
         'codellama-34b-instruct': codellama_34b_instruct,
         'codellama-70b-instruct': codellama_70b_instruct,
 
         # GigaChat
         'gigachat'     : gigachat,
         'gigachat_plus': gigachat_plus,
         'gigachat_pro' : gigachat_pro,
-
+        
+        # Mistral Opensource
         'mixtral-8x7b': mixtral_8x7b,
         'mistral-7b': mistral_7b,
         'mistral-7b-v02': mistral_7b_v02,
-        # 'mixtral-8x22b': mixtral_8x22b,
+        'mixtral-8x22b': mixtral_8x22b,
         'dolphin-mixtral-8x7b': dolphin_mixtral_8x7b,
-        'lzlv-70b': lzlv_70b,
-        'airoboros-70b': airoboros_70b,
-        'openchat_3.5': openchat_35,
+        
+        # google gemini
         'gemini': gemini,
         'gemini-pro': gemini_pro,
+        
+        # anthropic
         'claude-v2': claude_v2,
         'claude-3-opus': claude_3_opus,
         'claude-3-sonnet': claude_3_sonnet,
+        
+        # other
+        'command-r+': command_r_plus,
+        'dbrx-instruct': dbrx_instruct,
+        'lzlv-70b': lzlv_70b,
+        'airoboros-70b': airoboros_70b,
+        'openchat_3.5': openchat_35,
         'pi': pi
     }
 
 _all_models = list(ModelUtils.convert.keys())
```

### Comparing `g4f-0.2.9.8/g4f/providers/base_provider.py` & `g4f-0.2.9.9/g4f/providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/providers/create_images.py` & `g4f-0.2.9.9/g4f/providers/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/providers/helper.py` & `g4f-0.2.9.9/g4f/providers/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/providers/retry_provider.py` & `g4f-0.2.9.9/g4f/providers/retry_provider.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,117 +8,147 @@
 from .. import debug
 from ..errors import RetryProviderError, RetryNoProviderError
 
 class RetryProvider(BaseRetryProvider):
     def __init__(
         self,
         providers: List[Type[BaseProvider]],
-        shuffle: bool = True
+        shuffle: bool = True,
+        single_provider_retry: bool = False,
+        max_retries: int = 3,
     ) -> None:
         """
         Initialize the BaseRetryProvider.
-
         Args:
             providers (List[Type[BaseProvider]]): List of providers to use.
             shuffle (bool): Whether to shuffle the providers list.
+            single_provider_retry (bool): Whether to retry a single provider if it fails.
+            max_retries (int): Maximum number of retries for a single provider.
         """
         self.providers = providers
         self.shuffle = shuffle
+        self.single_provider_retry = single_provider_retry
+        self.max_retries = max_retries
         self.working = True
         self.last_provider: Type[BaseProvider] = None
 
-    """
-    A provider class to handle retries for creating completions with different providers.
-
-    Attributes:
-        providers (list): A list of provider instances.
-        shuffle (bool): A flag indicating whether to shuffle providers before use.
-        last_provider (BaseProvider): The last provider that was used.
-    """
     def create_completion(
         self,
         model: str,
         messages: Messages,
         stream: bool = False,
-        **kwargs
+        **kwargs,
     ) -> CreateResult:
         """
         Create a completion using available providers, with an option to stream the response.
-
         Args:
             model (str): The model to be used for completion.
             messages (Messages): The messages to be used for generating completion.
             stream (bool, optional): Flag to indicate if the response should be streamed. Defaults to False.
-
         Yields:
             CreateResult: Tokens or results from the completion.
-
         Raises:
             Exception: Any exception encountered during the completion process.
         """
         providers = [p for p in self.providers if stream and p.supports_stream] if stream else self.providers
         if self.shuffle:
             random.shuffle(providers)
 
         exceptions = {}
         started: bool = False
-        for provider in providers:
+
+        if self.single_provider_retry and len(providers) == 1:
+            provider = providers[0]
             self.last_provider = provider
-            try:
-                if debug.logging:
-                    print(f"Using {provider.__name__} provider")
-                for token in provider.create_completion(model, messages, stream, **kwargs):
-                    yield token
+            for attempt in range(self.max_retries):
+                try:
+                    if debug.logging:
+                        print(f"Using {provider.__name__} provider (attempt {attempt + 1})")
+                    for token in provider.create_completion(model, messages, stream, **kwargs):
+                        yield token
                     started = True
-                if started:
-                    return
-            except Exception as e:
-                exceptions[provider.__name__] = e
-                if debug.logging:
-                    print(f"{provider.__name__}: {e.__class__.__name__}: {e}")
-                if started:
-                    raise e
+                    if started:
+                        return
+                except Exception as e:
+                    exceptions[provider.__name__] = e
+                    if debug.logging:
+                        print(f"{provider.__name__}: {e.__class__.__name__}: {e}")
+                    if started:
+                        raise e
+        else:
+            for provider in providers:
+                self.last_provider = provider
+                try:
+                    if debug.logging:
+                        print(f"Using {provider.__name__} provider")
+                    for token in provider.create_completion(model, messages, stream, **kwargs):
+                        yield token
+                    started = True
+                    if started:
+                        return
+                except Exception as e:
+                    exceptions[provider.__name__] = e
+                    if debug.logging:
+                        print(f"{provider.__name__}: {e.__class__.__name__}: {e}")
+                    if started:
+                        raise e
 
         raise_exceptions(exceptions)
 
     async def create_async(
         self,
         model: str,
         messages: Messages,
-        **kwargs
+        **kwargs,
     ) -> str:
         """
         Asynchronously create a completion using available providers.
-
         Args:
             model (str): The model to be used for completion.
             messages (Messages): The messages to be used for generating completion.
-
         Returns:
             str: The result of the asynchronous completion.
-
         Raises:
             Exception: Any exception encountered during the asynchronous completion process.
         """
         providers = self.providers
         if self.shuffle:
             random.shuffle(providers)
 
         exceptions = {}
-        for provider in providers:
+
+        if self.single_provider_retry and len(providers) == 1:
+            provider = providers[0]
             self.last_provider = provider
-            try:
-                return await asyncio.wait_for(
-                    provider.create_async(model, messages, **kwargs),
-                    timeout=kwargs.get("timeout", 60)
-                )
-            except Exception as e:
-                exceptions[provider.__name__] = e
-                if debug.logging:
-                    print(f"{provider.__name__}: {e.__class__.__name__}: {e}")
+            for attempt in range(self.max_retries):
+                try:
+                    if debug.logging:
+                        print(f"Using {provider.__name__} provider (attempt {attempt + 1})")
+                    return await asyncio.wait_for(
+                        provider.create_async(model, messages, **kwargs),
+                        timeout=kwargs.get("timeout", 60),
+                    )
+                except Exception as e:
+                    exceptions[provider.__name__] = e
+                    if debug.logging:
+                        print(f"{provider.__name__}: {e.__class__.__name__}: {e}")
+        else:
+            for provider in providers:
+                self.last_provider = provider
+                try:
+                    if debug.logging:
+                        print(f"Using {provider.__name__} provider")
+                    return await asyncio.wait_for(
+                        provider.create_async(model, messages, **kwargs),
+                        timeout=kwargs.get("timeout", 60),
+                    )
+                except Exception as e:
+                    exceptions[provider.__name__] = e
+                    if debug.logging:
+                        print(f"{provider.__name__}: {e.__class__.__name__}: {e}")
 
         raise_exceptions(exceptions)
 
 class IterProvider(BaseRetryProvider):
     __name__ = "IterProvider"
 
     def __init__(
```

### Comparing `g4f-0.2.9.8/g4f/providers/types.py` & `g4f-0.2.9.9/g4f/providers/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/requests/__init__.py` & `g4f-0.2.9.9/g4f/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/requests/aiohttp.py` & `g4f-0.2.9.9/g4f/requests/aiohttp.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/requests/curl_cffi.py` & `g4f-0.2.9.9/g4f/requests/curl_cffi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/requests/defaults.py` & `g4f-0.2.9.9/g4f/requests/defaults.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/requests/raise_for_status.py` & `g4f-0.2.9.9/g4f/requests/raise_for_status.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/stubs.py` & `g4f-0.2.9.9/g4f/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/typing.py` & `g4f-0.2.9.9/g4f/typing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/version.py` & `g4f-0.2.9.9/g4f/version.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f/webdriver.py` & `g4f-0.2.9.9/g4f/webdriver.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f.egg-info/PKG-INFO` & `g4f-0.2.9.9/g4f.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.2.9.8
+Version: 0.2.9.9
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
@@ -355,14 +355,24 @@
 | [chatgpt.ai](https://chatgpt.ai) | `g4f.Provider.ChatgptAi` | ❌ | ✔️ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
 | [liaobots.site](https://liaobots.site) | `g4f.Provider.Liaobots` | ✔️ | ✔️ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
 | [chat.openai.com](https://chat.openai.com) | `g4f.Provider.OpenaiChat` | ✔️ | ❌ | ✔️ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | ✔️ |
 | [raycast.com](https://raycast.com) | `g4f.Provider.Raycast` | ✔️ | ✔️ | ✔️ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | ✔️ |
 | [beta.theb.ai](https://beta.theb.ai) | `g4f.Provider.Theb` | ✔️ | ✔️ | ✔️ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | ❌ |
 | [you.com](https://you.com) | `g4f.Provider.You` | ✔️ | ✔️ | ✔️ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | ❌ |
 
+## Best OpenSource Models
+While we wait for gpt-5, here is a list of new models that are at least better than gpt-3.5-turbo. **Some are better than gpt-4**. Expect this list to grow.
+
+| Website | Provider |  parameters | better than |
+| ------  | -------  |  ------ |  ------ | 
+| [mixtral-8x22b](https://huggingface.co/mistral-community/Mixtral-8x22B-v0.1) | `g4f.Provider.DeepInfra` | 176B / 44b active | gpt-3.5-turbo |
+| [dbrx-instruct](https://www.databricks.com/blog/introducing-dbrx-new-state-art-open-llm) | `g4f.Provider.DeepInfra` | 132B / 36B active| gpt-3.5-turbo |
+| [command-r+](https://txt.cohere.com/command-r-plus-microsoft-azure/) | `g4f.Provider.HuggingChat` | 104B | gpt-4-0613 |
+
+
 ### GPT-3.5
 
 | Website | Provider | GPT-3.5 | GPT-4 | Stream | Status | Auth |
 | ------  | -------  | ------- | ----- | ------ | ------ | ---- |
 | [chat3.aiyunos.top](https://chat3.aiyunos.top/) | `g4f.Provider.AItianhuSpace` | ✔️ | ❌ | ✔️ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | ❌ |
 | [chatforai.store](https://chatforai.store) | `g4f.Provider.ChatForAi` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
 | [chatgpt4online.org](https://chatgpt4online.org) | `g4f.Provider.Chatgpt4Online` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.2.9.8 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.2.9.9 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
@@ -193,15 +193,24 @@
 [chat.openai.com](https://chat.openai.com) | `g4f.Provider.OpenaiChat` | âï¸
 | â | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | âï¸
 | | [raycast.com](https://raycast.com) | `g4f.Provider.Raycast` | âï¸ |
 âï¸ | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) |
 âï¸ | | [beta.theb.ai](https://beta.theb.ai) | `g4f.Provider.Theb` | âï¸
 | âï¸ | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | â
 | | [you.com](https://you.com) | `g4f.Provider.You` | âï¸ | âï¸ | âï¸
-| ![Unknown](https://img.shields.io/badge/Unknown-grey) | â | ### GPT-3.5 |
+| ![Unknown](https://img.shields.io/badge/Unknown-grey) | â | ## Best
+OpenSource Models While we wait for gpt-5, here is a list of new models that
+are at least better than gpt-3.5-turbo. **Some are better than gpt-4**. Expect
+this list to grow. | Website | Provider | parameters | better than | | ------ |
+------- | ------ | ------ | | [mixtral-8x22b](https://huggingface.co/mistral-
+community/Mixtral-8x22B-v0.1) | `g4f.Provider.DeepInfra` | 176B / 44b active |
+gpt-3.5-turbo | | [dbrx-instruct](https://www.databricks.com/blog/introducing-
+dbrx-new-state-art-open-llm) | `g4f.Provider.DeepInfra` | 132B / 36B active|
+gpt-3.5-turbo | | [command-r+](https://txt.cohere.com/command-r-plus-microsoft-
+azure/) | `g4f.Provider.HuggingChat` | 104B | gpt-4-0613 | ### GPT-3.5 |
 Website | Provider | GPT-3.5 | GPT-4 | Stream | Status | Auth | | ------ | ----
 --- | ------- | ----- | ------ | ------ | ---- | | [chat3.aiyunos.top](https://
 chat3.aiyunos.top/) | `g4f.Provider.AItianhuSpace` | âï¸ | â | âï¸ | !
 [Unknown](https://img.shields.io/badge/Unknown-grey) | â | |
 [chatforai.store](https://chatforai.store) | `g4f.Provider.ChatForAi` | âï¸
 | â | âï¸ | ![Active](https://img.shields.io/badge/Active-brightgreen) |
 â | | [chatgpt4online.org](https://chatgpt4online.org) |
```

### Comparing `g4f-0.2.9.8/g4f.egg-info/SOURCES.txt` & `g4f-0.2.9.9/g4f.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/g4f.egg-info/requires.txt` & `g4f-0.2.9.9/g4f.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.8/setup.py` & `g4f-0.2.9.9/setup.py`

 * *Files identical despite different names*


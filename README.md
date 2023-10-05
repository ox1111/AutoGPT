# 설치 참고 : https://wikidocs.net/198402
'''bash
git clone -b stable https://github.com/Significant-Gravitas/Auto-GPT.git
cd Auto-GPT
pip install -r requirements.txt

cp .env.template .env


.env 작성

.env 파일 생성

다음 명령을 실행.

cp .env.template .env
OpenAI API 키 설정

OpenAI API 키를 발급받고 복사
.env 파일에서 OPENAI_API_KEY=로 시작하는 행을 찾아 자신의 OpenAI API 키를 기재
구글 API 키와 커스텀 서치 ID 설정

구글 API 키 설정
Google Cloud Console에서 프로젝트를 생성
https://console.cloud.google.com/

API 키 생성
.env 파일의 GOOGLE_API_KEY= 뒷부분에 자신의 구글 API 키를 기재
구글 커스텀 서치 설정
Custom Search API 활성화
https://cse.google.com/cse/all
Custom Search Engine에서 새 검색엔진을 만들고 검색엔진 ID를 복사
검색엔진 ID를 .env 파일의 CUSTOM_SEARCH_ENGINE_ID= 뒤에 붙여 넣음.
[선택 사항] 로컬 명령어 실행 허가

Auto-GPT가 파이썬 코드 이외의 로컬 명령어를 실행하도록 허가하려면 .env 파일의 EXECUTE_LOCAL_COMMANDS를 True로 바꾸고 주석을 해제한다.

EXECUTE_LOCAL_COMMANDS=True
※ Auto-GPT를 실행하면 메모리 파일([프로젝트 홈]/autogpt/auto/auto_gpt_workspace/auto-gpt.json)이 자동으로 만들어지므로 설치 시 따로 작업할 필요가 없다.


python -m autogpt

다음 그림과 같이 공지사항(NEWS) 아래에 I want Auto-GPT to:라는 프롬프트가 나온다. 이곳에 원하는 것을 입력하면 된다.


google 클라우드 api 키 만들기

https://cloud.google.com/docs/authentication/api-keys?hl=ko




'''

# 🌟 AutoGPT: the heart of the open-source agent ecosystem

[![Discord Follow](https://dcbadge.vercel.app/api/server/autogpt?style=flat)](https://discord.gg/autogpt) [![GitHub Repo stars](https://img.shields.io/github/stars/Significant-Gravitas/AutoGPT?style=social)](https://github.com/Significant-Gravitas/AutoGPT/stargazers) [![Twitter Follow](https://img.shields.io/twitter/follow/auto_gpt?style=social)](https://twitter.com/Auto_GPT) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**AutoGPT** is your go-to toolkit for supercharging agents. With its modular and extensible framework, you're empowered to focus on:

- 🏗️ **Building** - Lay the foundation for something amazing.
- 🧪 **Testing** - Fine-tune your agent to perfection.
- 👀 **Viewing** - See your progress come to life.

Be part of the revolution! **AutoGPT** stays at the forefront of AI innovation, featuring the codebase for the reigning champion in the Open-Source ecosystem.

---

<p align="center">
  <a href="https://lablab.ai/event/autogpt-arena-hacks">
    <img src="https://lablab.ai/_next/image?url=https%3A%2F%2Fstorage.googleapis.com%2Flablab-static-eu%2Fimages%2Fevents%2Fcll6p5cxj0000356zslac05gg%2Fcll6p5cxj0000356zslac05gg_imageLink_562z1jzj.jpg&w=1080&q=75" alt="AutoGPT Arena Hacks Hackathon" />
  </a>
</p>
<p align="center">
  <strong>We're hosting a Hackathon!</strong>
  <br>
  Click the banner above for details and registration!
</p>

---

## 🥇 Current Best Agent: AutoGPT

Among our currently benchmarked agents, AutoGPT scores the best. This will change after the hackathon - the top-performing generalist agent will earn the esteemed position as the primary AutoGPT 🎊

📈 To enter, submit your benchmark run through the UI.

## 🌟 Quickstart

- **To build your own agent** and to be eligible for the hackathon, follow the quickstart guide [here](https://github.com/Significant-Gravitas/AutoGPT/blob/master/autogpts/forge/tutorials/001_getting_started.md). This will guide you through the process of creating your own agent and using the benchmark and user interface.

- **To activate the best agent** follow the guide [here](https://github.com/Significant-Gravitas/AutoGPT/blob/master/autogpts/autogpt/README.md).

Want to build your own groundbreaking agent using AutoGPT? 🛠️ There are three major components to focus on:

### 🏗️ the Forge

**Forge your future!** The `forge` is your innovation lab. All the boilerplate code is already handled, letting you channel all your creativity into building a revolutionary agent. It's more than a starting point, it's a launchpad for your ideas. All tutorials are located [here](https://github.com/Significant-Gravitas/AutoGPT/tree/master/autogpts/forge/tutorials).

📘 [Learn More](https://github.com/Significant-Gravitas/AutoGPT/tree/master/autogpts/forge)

### 🎯 the Benchmark

**Test to impress!** The `benchmark` offers a stringent testing environment. Our framework allows for autonomous, objective performance evaluations, ensuring your agents are primed for real-world action.

📘 [Learn More](https://github.com/Significant-Gravitas/AutoGPT/blob/master/benchmark)

### 🎮 the UI

**Take Control!** The `frontend` is your personal command center. It gives you a user-friendly interface to control and monitor your agents, making it easier to bring your ideas to life.

📘 [Learn More](https://github.com/Significant-Gravitas/AutoGPT/tree/master/frontend)

---

### 🔄 Agent Protocol

🔌 **Standardize to Maximize!** To maintain a uniform standard and ensure seamless compatibility, AutoGPT employs the [agent protocol](https://agentprotocol.ai/) from the AI Engineer Foundation. This standardizes the communication pathways from your agent to the frontend and benchmark.

### 🤔 Questions? Problems? Suggestions?

#### Get help - [Discord 💬](https://discord.gg/autogpt)

[![Join us on Discord](https://invidget.switchblade.xyz/autogpt)](https://discord.gg/autogpt)

To report a bug or request a feature, create a [GitHub Issue](https://github.com/Significant-Gravitas/AutoGPT/issues/new/choose). Please ensure someone else hasn’t created an issue for the same topic.

<p align="center">
  <a href="https://star-history.com/#Significant-Gravitas/AutoGPT&Date">
    <img src="https://api.star-history.com/svg?repos=Significant-Gravitas/AutoGPT&type=Date" alt="Star History Chart">
  </a>
</p>

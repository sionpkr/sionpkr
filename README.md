# Sion Park

AI engineer working on model development, evaluation, and deployment, with a background in Python backend and full-stack web services.

I work on edge AI systems: choosing models from measured data, validating them against evaluation criteria, and deploying them safely on real devices. I also build and operate web services end to end, including the backend, database, AI integrations, and deployment.

Outside my main field, I built [tourney-method](https://tourneymethod.com/), an osu! tournament archive and community contribution platform. I had no PHP or Laravel experience when I started, so I learned the stack from documentation and AI coding agents, then built the service and now run it publicly.

[GitHub](https://github.com/sionpkr) | [LinkedIn](https://www.linkedin.com/in/sion-park-4717602a6/) | [Email](mailto:pso9809@gmail.com)

## What I bring

- In a domain I do not know yet, I start from the service flow and use documentation, existing code, and AI tools, while I stay responsible for direction, review, and validation.
- A problem I have solved once becomes reusable structure, so the next project does not start from zero.
- I take work from design through deployment and maintenance, and I say what has and has not been measured.

## AI and MLOps

I develop models in Python with PyTorch and scikit-learn. Candidate models run under the same protocol, data is split by test or event to avoid leakage, and the choice rests on recall and false-alarm numbers. I prefer measured data to synthetic data and write the limits next to the results.

For deployment I use ONNX and Hailo on Raspberry Pi, systemd services, signed releases with rollback, and human-approved model promotion. Around that sit test-driven development, evaluation gates before release, reusable project templates, and written decisions. I use AI coding agents such as Claude Code and review what they produce.

## Skills

Operating systems

![OS](https://skillicons.dev/icons?i=linux,windows,raspberrypi)

Languages

![Languages](https://skillicons.dev/icons?i=python,php,typescript,javascript,c,cpp)

AI and data

![AI](https://skillicons.dev/icons?i=pytorch,sklearn,tensorflow,opencv)

Frameworks

![Frameworks](https://skillicons.dev/icons?i=django,flask,laravel,nextjs,react,tailwind)

Development environments

![IDE](https://skillicons.dev/icons?i=vscode,visualstudio)

Databases and tools

![Others](https://skillicons.dev/icons?i=mysql,postgres,mongodb,redis,docker,aws,githubactions,git,nginx)

## Featured projects

### [tourney-method](https://github.com/sionpkr/tourney-method)

A live platform for finding osu! tournaments, browsing tournament history, and contributing community records.

This is outside my main field of AI and machine learning. I built it with AI coding agents and documentation, in a stack I had not used before.

- Built and operate [tourneymethod.com](https://tourneymethod.com/), with 1,000 logged-in users and active use in the osu! community.
- Plan the features, choose the technical approach, and design how community members contribute.
- Support tournament discovery, player and staff history, participation records, metadata corrections, multiple languages, and notifications.
- Maintain queue monitoring, backups, and health checks.
- Use AI coding agents to help with implementation, while taking responsibility for technical direction, code review, integration, and validation.

Built with Laravel 12, PostgreSQL, Redis, Livewire, Alpine.js, Tailwind CSS, Docker Compose, and Railway. Development tools include Pest, PHPStan, and Pint.

Community translations live in [tourney-method-locales](https://github.com/sionpkr/tourney-method-locales).

### [AICI / KT AIVLE School VOC TM](https://github.com/sionpkr/AICI_WEB)

A Django service for managing customer service (VOC) TM results and external construction reports, built during a company collaboration at KT AIVLE School.

- Led backend development and database design.
- Built authentication, role-based access control, construction and TM response status tracking, notices, and map-based construction information.
- Integrated AI models for speech-to-text, summarization, issue resolution detection, text correction, date and number formatting, and keyword extraction.
- Used my CS/VOC domain knowledge to clarify service workflows, establish shared terminology, and help the team decide what to build.
- Helped coordinate Git collaboration during backend and frontend integration. The team made over 200 commits in about two weeks.
- Received the Top Award among 50 participating teams.

### [Alyac Search / alyac_detect](https://github.com/sionpkr/alyac_detect)

A Python backend prototype for identifying pills from images and text.

- Built an API that reads text from uploaded images and returns matching pill data as JSON.
- Used Flask with flask-restx for the REST API, EasyOCR for text recognition, and a public pill dataset.
- Filtered relevant object contours before inference to reduce unnecessary model work.
- Reported an 89.5% improvement in model processing speed through preprocessing and filtering.

## Tech stack

- AI and data: Python, PyTorch, scikit-learn, TensorFlow, ONNX, MLflow, Hailo, OpenCV, pandas, SQL, machine learning, deep learning, computer vision, NLP, web crawling, Roboflow
- Backend: Python, Django, Flask, REST API, PHP, Laravel, MySQL, PostgreSQL, MongoDB
- Frontend and apps: JavaScript, TypeScript, Next.js, HTML, CSS, React Native, Livewire, Alpine.js, Tailwind CSS, PyQt5
- Infrastructure and development: Linux, systemd, Docker, Docker Compose, Git, GitHub, GitHub Actions, AWS, Gunicorn, Nginx, Redis, Railway, Vite, pytest, Pest, PHPStan, Pint

## How I work

I also learn from conversations with users and communities, and I turn that understanding into specifications, flowcharts, and shared terminology so the team can agree on what to build. I use spec-driven development and AI coding agents, and I review and integrate the results myself.

I keep decisions and implementation notes in writing, using Git and issue-style planning to make the work easier to follow.

## Current focus

I'm focused on edge AI model development and deployment: building the evaluation and release practices around the models, and measuring before optimizing. I keep operating tourney-method in production while deepening my Python, PyTorch, and Linux deployment skills. I'm also refining how I use AI coding agents, particularly how I write specifications, review their work, and validate changes.

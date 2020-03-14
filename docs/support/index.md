# 지원

엔진을 사용하는데 문제가 생겼을 경우 엔진의 패키지가 가장 최신버전인지 확인하시길 바랍니다. 패키지 업데이트는 [Asset Store window](https://docs.unity3d.com/Manual/AssetStore.html)를 통해 진행하실 수 있습니다.  
확장 패키지를 사용중이실 경우, 다음 링크에서 가장 최신 버전을 설치하시길 바랍니다.

- [NaninovelLive2D](https://github.com/Elringus/NaninovelLive2D/raw/master/NaninovelLive2D.unitypackage)
- [NaninovelPlayMaker](https://github.com/Elringus/NaninovelPlayMaker/raw/master/NaninovelPlayMaker.unitypackage)
- [NaninovelAdventureCreator](https://github.com/Elringus/NaninovelAdventureCreator/raw/master/NaninovelAdventureCreator.unitypackage)

업데이트를 시도했음에도 문제가 해결되지 않을 경우, 재설치를 시도해 보시길 바랍니다.  
재설치는 `Naninovel` 폴더를 프로젝트에서 삭제 후 Asset Store에서 다시 임포팅함으로서 진행할 수 있습니다.

패키지를 지우거나 업데이트를 하실 때 **항상 백업 또는 [버전 컨트롤 서비스](https://en.wikipedia.org/wiki/Version_control)를** 사용 하시길 바랍니다. 신 조차도 이 작업 중에 어떤일이 일어날지 알 수 없기 때문입니다. `ʕノ•ᴥ•ʔノ ︵ ┻━┻`

## 이슈 트래커

위의 내용을 진행했음에도 문제가 해결되지 않을 경우, [issue tracker](https://github.com/Elringus/NaninovelWeb/issues?q=is%3Aissue+label%3Abug)를 확인하십시오. 이미 해당 버그가 수정중일 수도 있습니다. 그렇지 않다면 [bug report](https://github.com/Elringus/NaninovelWeb/issues/new?labels=bug&template=bug_report.md)를 통해 제보해 주시면 감사하겠습니다.(English Only)

## 개발자 지원

직접 개발자 지원을 받으려면 [Discord 서버](https://discord.gg/BfkNqem)<svg xmlns="http://www.w3.org/2000/svg" aria-hidden="true" x="0px" y="0px" viewBox="0 0 100 100" width="15" height="15" class="icon outbound"><path fill="currentColor" d="M18.8,85.1h56l0,0c2.2,0,4-1.8,4-4v-32h-8v28h-48v-48h28v-8h-32l0,0c-2.2,0-4,1.8-4,4v56C14.8,83.3,16.6,85.1,18.8,85.1z"></path> <polygon fill="currentColor" points="45.7,48.7 51.3,54.3 77.2,28.5 77.2,37.2 85.2,37.2 85.2,14.9 62.8,14.9 62.8,22.9 71.5,22.9"></polygon></svg>에 가입하고, [다음 양식](https://naninovel.com/register/)<svg xmlns="http://www.w3.org/2000/svg" aria-hidden="true" x="0px" y="0px" viewBox="0 0 100 100" width="15" height="15" class="icon outbound"><path fill="currentColor" d="M18.8,85.1h56l0,0c2.2,0,4-1.8,4-4v-32h-8v28h-48v-48h28v-8h-32l0,0c-2.2,0-4,1.8-4,4v56C14.8,83.3,16.6,85.1,18.8,85.1z"></path> <polygon fill="currentColor" points="45.7,48.7 51.3,54.3 77.2,28.5 77.2,37.2 85.2,37.2 85.2,14.9 62.8,14.9 62.8,22.9 71.5,22.9"></polygon></svg>을 채워 에셋구매 인증을 하시길 바랍니다. 

인증 후에는 자동으로"Verified User" role을 부여 받아 `#support` 체널에 접근하실 수 있게 됩니다. 또한, 개발자인 `@Elringus#6359` 에게 개인적으로 질문도 할 수 있습니다.

<iframe src="https://discordapp.com/widget?id=545676116871086080&theme=dark" width="100%" height="500" allowtransparency="true" frameborder="0"></iframe>

## 프로젝트 재가공

우리는 issue를 보고받을 때, "repro" 프로젝트를 공유하라고 요구할 수 있습니다. repro프로젝트는 꺠끗하고 완전히 새로운 Unity프로젝트여야 하며, 문제를 재현하는데 필요한 **가장 최소한의** 수정내용과 추가 에셋만을 포함해야 합니다.

다음과 같은 단계를 통해 프로젝트를 재가공하여 공유하십시오.

1. 새로운 유니티 프로젝트를 만들어주십시오. 프로젝트를 만들 때는 사용중인 유니티 버전이 [최신 Naninovel의 버전](https://github.com/Elringus/NaninovelWeb/releases)과 호환되는지 확인하셔야 합니다.
2. 가장 최신의 Naninovel을 임포팅합시오. (pre-release버전이 존재한다면 그 버전을 대신 사용하십시오.)
3. 필요한 에셋들을 임포팅하고, 프로젝트를 수정하여 문제를 재현하십시오. Naninovel 스크립트는 반드시 짧게 유지하고, 문제를 재현하는데 필수적인 에셋만 포함해야만 합니다.
4. 유니티에디터를 닫고 프로젝트의 루트폴더로 이동하여 `Assets`, `Packages`, `ProjectSettings`들을 제외한 나머지 파일을 모두 지우십시오. 특히, 자동으로 생성된 파일이 많이 존재하는 **`Library` 폴더가 지워졌는지 확인하는 것이 가장 중요합니다.**
5. zip확장자로 프로젝트파일을 압축하여 Google Drive에 업로드하거나 Discord 개인 메세지에 첨부하십시오.

프로젝트를 공유하실 때 프로젝트 파일과 같이 아래처럼 문제 재현 단계를 명시해야 합니다.

>번역 전 원본 예시 (issue를 보고할 땐 반드시 영어로 작성해야 합니다.)
```
1. Open "SampleScene".
2. Enter play mode in the editor.
3. Start a new game.
4. Play through to the line number 15.
5. Save and load the game.
```
>번역 후 예시
```
1. "SampleScene"을 연다.
2. 유니티에디터에서 게임실행 모드에 들어 간다.
3. 게임을 테스트하기 위해 실행한다.
4. 15번 스크립트 라인을 지난다.
5. 저장 후 게임을 로드 합니다.
```
<br>
재현 단계 명시 후 예상했던 결과와 실제 실행 결과를 같이 작성합니다.  
>번역 전 원본 예시 (issue를 보고할 땐 반드시 영어로 작성해야 합니다.)

```
Expected: Music "Ambient" should start playing.
Actual: No music is playing.
```
>번역 후 예시
```
예상한 결과: 음원"Ambient"가 재생되어야 한다.
실제 결과: 음원이 재생되지 않는다.
```

경고. 재생산된 프로젝트는 반드시 **개인 메세지로** 보내십시오. 공개 체널에는 절대로 파일을 업로드해서는 안됩니다.
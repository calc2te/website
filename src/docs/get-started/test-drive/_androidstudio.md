<div class="tab-pane active" id="androidstudio" role="tabpanel" aria-labelledby="androidstudio-tab" markdown="1">

## 앱 생성 {#create-app}

 1. IDE를 켜고 **Start a new Flutter project**를 선택하세요.
 1. 프로젝트 타입으로 **Flutter Application**을 선택하세요. **Next**을 누르세요.
 1. SDK의 위치에 맞게 경로가 설정되어 있는지 확인하세요 (텍스트 필드가 비어 있으면 **Install SDK...**를 선택하세요).
 1. 프로젝트 이름을 입력하세요 (예, `myapp`). 그런 다음 **Next**를 누르세요.
 1. **Finish**를 클릭하세요.
 1. Android 스튜디오가 SDK를 설치하고 프로젝트를 생성할 때까지 기다리세요.

{{site.alert.note}}
  새로운 Flutter 앱을 생성할 때, 특정 Flutter IDE 플러그인이
  회사 도메인 이름을 `com.example`와 같이 역순으로 요청할 수 있습니다.
  회사 도메인 이름과 프로젝트 이름을 합쳐서 앱을 출시할 때 
  Android 패키지 이름(iOS 번들 ID)으로 사용됩니다.
  앱을 출시할 예정이면, 지금 
  패키지 이름을 정확히 정하는 게 좋습니다.
  패키지 이름은 앱이 출시되면 바꿀 수 없으므로
  고유한 이름으로 지정하세요.
{{site.alert.end}}

위 명령은 [머티리얼 컴포넌트][]를 사용한 간단한 예시 앱이 들어있는 Flutter 프로젝트 디렉토리 `myapp`을 생성합니다.

{% include_relative _main-code-note.md  %}

## 앱 실행

 1. Android 스튜디오 기본 툴바를 찾으세요: <br>
    ![Main IntelliJ toolbar][]{:.mw-100}
 1. **target selector**에서, 앱을 실행할 Android 기기를 선택하세요.
    리스트에 사용 가능한 기기가 없다면, 
    **Tools> Android > AVD Manager**를 선택하고 새 기기를 생성하세요.
    자세한 사항은, [AVD 관리][]를 참조하세요.
 1. 툴바에서 실행 아이콘을 선택하세요, 
    또는 메뉴 항목에서 **Run > Run**를 실행하세요.

{% capture save_changes -%}
  : invoke **Save All**, or click **Hot Reload**
  <i class="material-icons align-bottom">offline_bolt</i>.
  {% comment %} Or, as an alternative:
    {% asset 'get-started/hot-reload-button.png' alt='looks like a lightning bolt' %}.
  {% endcomment -%}
{% endcapture %}

{% capture ide_profile -%}
  to invoke the menu item **Run > Profile** in the IDE, or
{% endcapture %}

{% include_relative _try-hot-reload.md save_changes=save_changes %}
{% include run-profile.md ide_profile=ide_profile %}

[Main IntelliJ toolbar]: {% asset tools/android-studio/main-toolbar.png @path %}
[AVD 관리]: {{site.android-dev}}/studio/run/managing-avds
[머티리얼 컴포넌트]: {{site.material}}/guidelines
</div>

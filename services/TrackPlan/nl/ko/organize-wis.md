---

 

copyright:

  years: 2015, 2016

 

---

{:shortdesc: .shortdesc}
{:screen: .screen}
{:new_window: target="_blank"}
{:codeblock: .codeblock}

#작업 항목 구성 및 필터링 {: #tp-organize}  

*마지막 업데이트 날짜: 2016년 4월 29일*
{: .last-updated}

{{site.data.keyword.trackplan}} 서비스에 작업 항목 정렬 및 구성을 위한 몇 가지 옵션이 있습니다.
{: shortdesc}

##작업 항목 필터링 {: #tp-filteringwis}

특정 속성에 대한 값 또는 단어를 기준으로 작업 항목을 필터링할 수 있습니다. 

필터링이 다음 보기에서 지원됩니다.   
- 내 작업
- 구독하는 내 작업
- 수신 작업
- 백로그
- 스프린트 플랜
- 팀 작업
- 모든 작업

단어를 입력하면 해당 단어가 포함된 작업 항목 요약이 표시됩니다. 또한 특정 속성의 값을 기준으로 작업 항목을 필터링할 수 있습니다. 세부사항은 다음 표를 참조하십시오.

|  속성  | 예제  | 
|-------|-------|
|*Type  | `*Defect` |
|#Tag  | `#conference`| 
|@:Owner  | `@:jasmith`|
|$Priority|`$High`|
|!Severity|`!Major`|       
   

속성 이름을 입력하여 작업 항목 속성을 사용하는 조회를 작성할 수 있습니다. 예를 들어, `Created by`를 입력하면 조회 옵션 및 구문이 표시됩니다. 필터 기준에 연산자(예: "and," "or," "not")을 사용할 수 있습니다. 또한 소괄호를 사용하여 여러 연산자를 중첩시키는 복합 연산을 포함할 수 있습니다. 예를 보려면 **도움말** 아이콘을 클릭하십시오.
![필터링 도움말 아이콘](images/filter_helpicon.png)

**키워드로 작업 항목 필터링** 필드를 클릭하면 조회를 작성하는 데 사용할 수 있는 연산자 및 필터가 표시됩니다.

![자동 완료 선택사항으로 필터링](images/filterMenu2.png)

##사용자 정의 보기 저장 {: #tp-customviews}
필터를 적용하여 사용자 정의 보기를 작성할 수 있습니다. 그런 다음 팀과 보기를 공유할 수 있습니다.    

1. **작업 항목 필터링** 필드에 속성 유형의 간단한 양식 및 해당 속성의 값을 입력하십시오(예: `$high`). 간단한 양식을 입력하면 일부 속성 선택사항이 자동으로 나열됩니다(예: *Type, $Priority, !Severity).
![속성 유형 및 속성으로 필터링](images/filterAttributes.png)
2. **저장**을 클릭하십시오.
3. 보기의 이름을 지정하십시오. 
4. 사용자 정의 보기에 보고 있는 스프린트를 포함하려면 선택란을 선택하여 스프린트를 포함하십시오. 다음 예에서 백로그 스프린트가 "높은 우선순위 백로그" 보기에 포함됩니다.
![스프린트가 포함된 사용자 정의 보기 대화 상자 저장](images/filterIncludeSprints.png)
5. **저장**을 클릭하십시오. 
6. 팀과 저장된 보기를 공유하려면 사용자 정의 보기 섹션에서 새 보기 옆에 있는 공유 아이콘을 클릭하십시오. 그런 다음 **확인**을 클릭하십시오.
![사용자 정의 보기 공유 화살표](images/filterShare.png)

사용자 정의 보기는 보고 있는 현재 스프린트 및 상태에 대한 결과만 리턴합니다. 보기에서 추가 스프린트 또는 상태에 대한 결과를 리턴하려면 보기를 클릭하여 필요에 따라 변경하십시오.

##작업 항목 보기 및 구성 {: #tp-organizingwis}

- 소유한 작업 항목을 보려면 내 작업 보기를 참조하십시오. 
- 특정 작업 항목을 자주 사용하는 경우 별 아이콘(<img class="inline"  src="./images/star.gif" alt="별 아이콘">)을 클릭하여 이 작업 항목을 즐겨찾기로 표시할 수 있습니다. 그런 다음, 즐겨찾기 된 내 작업 보기에서 즐겨찾기 작업 항목을 모두 볼 수 있습니다. 사용자가 작업 항목에 대해 별 아이콘을 클릭하면 이 사용자만 작업 항목이 즐겨찾기로 표시된 것을 볼 수 있습니다.  
- 구독하는 모든 작업 항목을 보려면 구독하는 내 작업 보기를 확인하십시오.
- 수정된 날짜를 기준으로 정렬된 작업 항목을 보려면 최근 내 작업 보기를 확인하십시오.
- 작업 항목 활동을 보려면 내 활동 보기를 확인하십시오. 내 이벤트 섹션에 사용자가 언급된 작업 항목이 나열됩니다. 내 구독 섹션에는 구독하는 작업 항목에서 발생한 모든 변경사항이 나열됩니다.

##작업 항목 선별 {: #tp-triaging}

작업 항목이 작성되었지만 스프린트에 지정되지 않은 경우 작업 항목이 수신 작업 보기에 표시됩니다.
작업 항목이 스프린트에 지정되자마자 수신 작업 보기에서 제거됩니다.

수신 작업 보기에서 다음 여러 가지 방법으로 작업 항목을 선별할 수 있습니다. 
- 작업 항목을 거부하려면 **이 항목을 휴지통에 버리기** 아이콘(<img class="inline"  src="./images/trash.gif" alt="이 항목을 휴지통에 버리기 아이콘">)을 클릭하십시오. 작업 항목이 분석되고 해당 상태가 올바르지 않음으로 변경됩니다.
- 작업 항목을 채택하고 백로그에 지정하려면 **백로그로 선별** 아이콘(<img  class="inline" src="./images/triage.gif" alt="백로그로 선별 아이콘">)을 클릭하십시오. 그런 다음 스프린트 플랜 보기에서 다른 작업 항목에 대해 작업 항목을 평가하고 스프린트에 작업 항목을 지정할 수 있습니다.
- 스프린트에 작업 항목을 지정하려면 작업 항목을 열고 **플랜 대상** 목록에서 값을 선택하십시오.

![수신 작업 보기에서 작업 항목 선별](images/incoming_work_attributes.png)  

작업 항목 관리에 대한 자세한 정보는 [Managing a project with Quick Planner를 참조하십시오](http://www.ibm.com/support/knowledgecenter/SSYMRC_6.0.1/com.ibm.team.concert.tutorial.doc/topics/tut_quick_planner_lesson.html).
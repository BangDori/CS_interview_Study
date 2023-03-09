# 우선순위 큐(Priority Queue)

# PriorityQueue란 무엇이며 동작 원리가 어떻게 되나요

- 우선순위 큐
    - 우선순위를 가진 데이터들을 저장하는 큐(Queue)
    - 데이터를 꺼낼 때 우선순위가 높은 데이터가 가장 먼저 나옴
    
    ![images_april_5_post_2347c105-c122-4173-8e90-4132283b3149_image.png](%E1%84%8B%E1%85%AE%E1%84%89%E1%85%A5%E1%86%AB%E1%84%89%E1%85%AE%E1%86%AB%E1%84%8B%E1%85%B1%20%E1%84%8F%E1%85%B2(Priority%20Queue)%20812425284dd2464296292dc50cccc671/images_april_5_post_2347c105-c122-4173-8e90-4132283b3149_image.png)
    
    - 일반적인 큐 vs 우선순위 큐
        - 일반적인 큐: 선형 구조
        - 우선순위 큐: 트리 구조, 최대 힙(Max Heap)을 이용
- 완전 이진트리
    
    ![Untitled](%E1%84%8B%E1%85%AE%E1%84%89%E1%85%A5%E1%86%AB%E1%84%89%E1%85%AE%E1%86%AB%E1%84%8B%E1%85%B1%20%E1%84%8F%E1%85%B2(Priority%20Queue)%20812425284dd2464296292dc50cccc671/Untitled.png)
    
    - 마지막 레벨을 제외 하고 모든 레벨이 완전히 채워져 있어야 함
    - 노드가 왼쪽에서 오른쪽으로 채워져야 함
- 최대 힙 (Max Heap)
    
    ![Untitled](%E1%84%8B%E1%85%AE%E1%84%89%E1%85%A5%E1%86%AB%E1%84%89%E1%85%AE%E1%86%AB%E1%84%8B%E1%85%B1%20%E1%84%8F%E1%85%B2(Priority%20Queue)%20812425284dd2464296292dc50cccc671/Untitled%201.png)
    
    ![Untitled](%E1%84%8B%E1%85%AE%E1%84%89%E1%85%A5%E1%86%AB%E1%84%89%E1%85%AE%E1%86%AB%E1%84%8B%E1%85%B1%20%E1%84%8F%E1%85%B2(Priority%20Queue)%20812425284dd2464296292dc50cccc671/Untitled%202.png)
    
    - 부모 노드가 자식 노드보다 값이 큰 완전 이진트리
    - 루트 노드는 전체 트리에서 가장 큰 값을 가짐
- 동작 구조
    - 삽입
        
        ![Untitled](%E1%84%8B%E1%85%AE%E1%84%89%E1%85%A5%E1%86%AB%E1%84%89%E1%85%AE%E1%86%AB%E1%84%8B%E1%85%B1%20%E1%84%8F%E1%85%B2(Priority%20Queue)%20812425284dd2464296292dc50cccc671/Untitled%203.png)
        
        ![images_april_5_post_9ce5454f-8e61-468e-bdae-08d3f6fb63fb_image.png](%E1%84%8B%E1%85%AE%E1%84%89%E1%85%A5%E1%86%AB%E1%84%89%E1%85%AE%E1%86%AB%E1%84%8B%E1%85%B1%20%E1%84%8F%E1%85%B2(Priority%20Queue)%20812425284dd2464296292dc50cccc671/images_april_5_post_9ce5454f-8e61-468e-bdae-08d3f6fb63fb_image.png)
        
        ![images_april_5_post_d363a7a2-dc48-4422-8b7d-ee95bd2e0a17_image.png](%E1%84%8B%E1%85%AE%E1%84%89%E1%85%A5%E1%86%AB%E1%84%89%E1%85%AE%E1%86%AB%E1%84%8B%E1%85%B1%20%E1%84%8F%E1%85%B2(Priority%20Queue)%20812425284dd2464296292dc50cccc671/images_april_5_post_d363a7a2-dc48-4422-8b7d-ee95bd2e0a17_image.png)
        
        ![images_april_5_post_9d1c9d5f-72ff-4ce7-950d-755f00283cee_image.png](%E1%84%8B%E1%85%AE%E1%84%89%E1%85%A5%E1%86%AB%E1%84%89%E1%85%AE%E1%86%AB%E1%84%8B%E1%85%B1%20%E1%84%8F%E1%85%B2(Priority%20Queue)%20812425284dd2464296292dc50cccc671/images_april_5_post_9d1c9d5f-72ff-4ce7-950d-755f00283cee_image.png)
        
    - 삭제
        
        ![images_april_5_post_94d288cc-8305-4faf-b6b7-8462458ea6df_image.png](%E1%84%8B%E1%85%AE%E1%84%89%E1%85%A5%E1%86%AB%E1%84%89%E1%85%AE%E1%86%AB%E1%84%8B%E1%85%B1%20%E1%84%8F%E1%85%B2(Priority%20Queue)%20812425284dd2464296292dc50cccc671/images_april_5_post_94d288cc-8305-4faf-b6b7-8462458ea6df_image.png)
        
        ![images_april_5_post_aed9127b-2bfd-415c-ac33-74d2afa9da99_image.png](%E1%84%8B%E1%85%AE%E1%84%89%E1%85%A5%E1%86%AB%E1%84%89%E1%85%AE%E1%86%AB%E1%84%8B%E1%85%B1%20%E1%84%8F%E1%85%B2(Priority%20Queue)%20812425284dd2464296292dc50cccc671/images_april_5_post_aed9127b-2bfd-415c-ac33-74d2afa9da99_image.png)
        
        ![images_april_5_post_4c7a20b7-bd34-4bc5-b564-627ae758d136_image.png](%E1%84%8B%E1%85%AE%E1%84%89%E1%85%A5%E1%86%AB%E1%84%89%E1%85%AE%E1%86%AB%E1%84%8B%E1%85%B1%20%E1%84%8F%E1%85%B2(Priority%20Queue)%20812425284dd2464296292dc50cccc671/images_april_5_post_4c7a20b7-bd34-4bc5-b564-627ae758d136_image.png)
        
- 답안
    - 우선순위 큐는 가장 우선순위가 높은 데이터를 먼저 꺼내기 위한 자료구조이며 완전이진트리를 이용한 힙을 사용하여 구현한다. 힙은 모든 정점이 자신의 자식요소보다 우선순위가 높다는 성질을 가지고 있다. 이 성질을 이용하여 O(logN)의 시간으로 삽입과 삭제연산을 수행할 수 있다.
- 질문
    1. Min Heap으로 구현할 수 있나요?
        
        → Min Heap도 상관은 없으나 숫자가 적은게 우선순위가 높다고 가정하여야 함
        
- 참고자료
    
    [[자료구조] 트리(Tree)의 개념 | 이진 트리,  전 이진 트리, 완전 이진트리, 포화 이진 트리, 이진 탐색트리](https://code-lab1.tistory.com/8)
    
    [🌈 자료구조:: 우선순위 큐(Priority Queue)](https://velog.io/@april_5/자료구조-우선순위-큐Priority-Queue)
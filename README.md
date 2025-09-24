# Recoil Root

Recoil 상태를 사용하는 컴포넌트는 부모 트리 어딘가에 나타나는 `RecoilRoot`가 필요하다.  
루트 컴포넌트가 `RecoilRoot`를 넣기에 가장 좋은 장소다.
---

# Atom

Atom은 상태(state)의 일부를 나타낸다. Atoms는 어떤 컴포넌트에서나 읽고 쓸 수 있다.  
atom의 값을 읽는 컴포넌트들은 암묵적으로 atom을 구독한다. 그래서 atom에 어떤 변화가 있으면 그 atom을 구독하는 모든 컴포넌트들이 재 렌더링 되는 결과가 발생할 것이다.
---

# Selector

Selector는 atom 혹은 다른 Selector 상태를 입력받아 동적인 데이터를 반환하는 순수 함수입니다.  
Selector가 참조하던 다른 상태가 변경되면 이도 같이 업데이트되며, 이때 Selector를 바라보던 컴포넌트들이 재 렌더링 되는 것이다.

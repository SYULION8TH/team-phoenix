Git에서 작업 되돌아가기
reset과 revert

Git reset
: 과거의 특정 커밋으로 이동하고, 이동 이후의 커밋은 삭제
이동 후 삭제된 커밋은 되돌릴 수 없으니 주의!

#git reset <옵션> <커밋ID>

옵션 : mixed(기본값) / hard / soft
- mixed : Index 초기화, 변경된 내용은 남겨둠
- hard : 변경 이력 및 내용 등 모두 초기화
- soft : 변경 이력은 삭제, 내용은 남겨둠

Git revert
: 과거의 특정 커밋으로 이동하지만 변경 내역은 유지
다른 사람들과 함께 작업할 때 유용!

#git revert <되돌릴 커밋>
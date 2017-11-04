# Notebooks Title
## section 1

Self Knowledge Management
test it

edit by zbo in 1st branch

现在来测试一下中文的情况再说

3-9行：
```
SYSTYPE            :=    $(shell uname)
ifneq ($(findstring CYGWIN, $(SYSTYPE)),) 
  MK_DIR := $(shell cygpath -m ../mk)
else
  MK_DIR := $(patsubst %/,%,$(dir $(lastword $(MAKEFILE_LIST))))
endif
```

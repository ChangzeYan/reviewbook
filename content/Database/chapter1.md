# 数据库
## 第一章

### 1.sql的执行顺序：
参考：https://wang286480403.iteye.com/blog/1899915
```yaml
1. from
2. on
3. join
4. where
5. group by
6. WITH {CUBE | ROLLUP} avg,sum...
7. having
8. select
9. distinct
10. order by
```

```yaml
1  (8)SELECT (9) DISTINCT (11) <TOP_specification> <select_list>
2  (1)  FROM <left_table>
3  (3) <join_type> JOIN <right_table>
4  (2) ON <join_condition>
5  (4) WHERE <where_condition>
6  (5) GROUP BY <group_by_list>
7  (6) WITH {CUBE | ROLLUP}
8  (7) HAVING <having_condition>
9 (10) ORDER BY <order_by_list>
```

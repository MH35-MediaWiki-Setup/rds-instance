# RDS instance
RDSインスタンスの定義

## 使い方

1. `aws cloudformation deploy --template-file formation.yml --stack-name [your stack name] --parameter-overrides Subnets=[private subnet IDs separated by commas] RdsSecurityGroup=[RDS subnet group ID] ParameterGroup=[RDS parameter group ID] OptionGroup=[RDS option group ID] AllocatedStorage=[RDS initial allocated storage size] MaxAllocatedStorage=[RDS maximum allocated storage size] InstanceType=[RDS instance type] DatabaseName=[Database name] DatabaseUser=[Database username] DatabasePassword=[Database password]`する
2. デプロイ完了まで待つ

## 作成されるもの

* RDSインスタンスおよびそれが所属するサブネットグループ

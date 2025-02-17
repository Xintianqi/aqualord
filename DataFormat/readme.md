# 数据格式

多维格式（包括 NetCDF、GRIB 和 HDF）常用于在科学社区中存储气象及海洋数据（如温度、湿度、风速和风向等）。数据通常以**变量的形式**进行存储，**每一个变量均为一个多维数组**。

这些数据格式方便了大批量地理时空数据的增删改查，且有相应的工具配合使用，本文件夹下就简单记录下这些常见的数据格式（日常积累中……）。

个人比较常见的多维栅格类型有：netCDF、GRIB 和 HDF，分别对应以这些格式存储的多维栅格数据。

- GRIB：常规二进制规则分布信息世界气象组织是一种简明的数据格式，在气象学中较为常用，用于存储历史及预报天气数据。GRIB 栅格类型可用于将 GRIB 1 和 GRIB 2 数据添加至镶嵌数据集中。要查看示例工作流，请参阅使用矢量字段模板创建镶嵌数据集。
- HDF：层次数据格式HDF 组是由美国国家超级计算应用中心 (NCSA) 设计用于存储科学数据的格式。HDF 栅格类型可用于将 HDF4 和 HDF5 中存储的栅格数据添加到镶嵌数据集中。HDF 文件中存储的非栅格数据将会被 HDF 栅格类型忽略。
- NetCDF：NetCDF（网络公用数据格式）是一种用于存储多维数据的文件格式。有关详细信息，请参阅 NetCDF 数据存储的基础知识。目前，netCDF 栅格类型支持气候和预测 (CF)CF 公约和元数据以及海洋/大气合作研究数据服务 (COARDS) 公约。采用其他约定创建的 NetCDF 文件也可用，但并不受 netCDF 栅格类型支持。要查看示例工作流，请参阅创建和可视化 netCDF 镶嵌数据集。

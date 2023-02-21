- 挂载106命令：

  > sudo sshfs -o allow_other hzy@10.0.1.206:/data5/Testing_Datasets/Uncut_Image/A200 206_A200_test/

- 卸载命令：

  > umount xxx/xx/xx/

- 创建文件夹：mkdir hzy

- 删除文件夹：rm -rf hzy

- 全部图片名写入list：find 206_A200_test/Fake_Face/ -name "*IRLeft.png" > A200_test.txt

- 追加写入上个list：find 206_A200_test/Live_Face/* -name "*IRLeft.png" >> A200_test.txt


- pip install -i https://pypi.tuna.tsinghua.edu.cn/simple xxx


- nautilus 查看当前文件夹

- 查看GPU的使用情况   循环监控：

  > watch -n 0.5 nvidia-smi

- 选择指定的GPU跑

  > CUDA_VISIBLE_DEVICES=2,3 python face_detection.py

- 当前目录下图片的数量 

  > ls -lR | grep "png" | wc -l
  >
  > -name *.png > count ; wc -l count

- 把相对路径写入 txt

  > find end_crop/ -name *png > crop_end.txt


- 查看txt总行数

  >wc -l ss.txt

- 选择多个文件夹，并把所有文件的相对路径写入txt中

  > 


����Ŀ����Tesseract V3.01�汾(V3.02�汾��ѵ��ʱ�иĶ�����shapeclustering����)

Tesseract�÷���
	���û�������TESSDATA_PREFIX =��D:\Tesseract-ocr\������tessdata��Ŀ¼����Դ���лᵽ���·���²�����Ӧ���ֿ��ļ�����ʶ��
	�����ʽ��tesseract imagename outputbase [-l lang] [-psm pagesegmode] [configfile...]
	ֻʶ�������
		tesseract imagename outputbase -l eng digits
	���empty page!!
		-psm N
		7 = Treat the image as a single text line
		tesseract imagename outputbase -l eng -psm 7
	configfile ����ֵΪtessdata\configs �� tessdata\tessconfigs Ŀ¼�µ��ļ���
		tesseract imagename outputbase -l eng nobatch

��֤��ʶ����Ŀʹ�÷���1��
	�����ص�ͼƬ�ŵ�./picĿ¼�£�
		��֤��ͼƬ���ƣ�get_random.jpg
		�۸�ͼƬ���ƣ�get_price_img.png
	�����ʽ��
		��֤��ͼƬʶ��python tess_test.py ./pic/get_random.jpg
		�۸�ͼƬʶ��python tess_test.py ./pic/get_price_img.png
	��ӡ��ʶ��Ľ������Ҫ�����������ʱ�ı��ļ�temp.txt�У����޸�pytessr_pro.py�д���"cleanup_scratch_flag = True"��Ϊ"cleanup_scratch_flag = False"
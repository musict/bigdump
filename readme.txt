������ ������� ��� MYSQL ����� BigDump

����� ��������� ������������� �������� ������� ��� ������ �� ������. ��� ����� ���� ��� ��������� �����, ��� � ������, ������������ � ������� ��������, ��� ��� �����-���� ��. 

������ �������� ������������ ��-����� ����������� ����������� ����������������� ���� � phpmyadmin. � ���� ���� ��� ����������� � ����������, � �������� �����, �������, ������, ������� �� ��� ������� ��������� ������� ���� ������ ����� ������� �� �����, �� ������ ������ ����������� ������������� ������� �����. ���� � ���, ��� ��-���������, ������������ ������ ������������ ����� ���������� � 2-100 ��. �����, ������� ��� ���������, �� ��� �����, ��� ����� ������� �� ���� ����� �� �������� ���������.

����� ����� ������������ ��� ����� ����� BigDump � ����������, � �������� ����� php-������, ���������� �������� ��������. ���� ������ ��������� � �������� ������ ��������� � ��������� ���� ��.

 
������� ���������� ��� ������������� - ������� 1:

1)      ������� BigDump - ��� http://www.ozerov.de/bigdump/

2)      ���������� ��������� ��, � ���� ������� � ��� - ������ ��������� ��� ���� ������ � ������� �� ��������� ��������� ������� ���� ������.

         ��� ����� �������, ������ � ��������� ����� ��������������� ������:

         $db_server   = 'localhost';    //������ ��

         $db_name     = '';                // �������� ��

         $db_username = '';            // ��� ������������ ��

         $db_password = '';             // ������

3)      ����������� ���� SQL � �� �� ����������, ��� � ��������� ������ BigDump, � ������� ��� ����� ����� � ���������� $filename.

4)      ������� ������������ ���������� ����� � ����� ������� � ���������� $linespersession (��-��������� ��� ����������� 300).

5)      ���������� ��������� ������ SQL-����� � ���������� $db_connection_charset (��������: �utf8�, �latin1�, �cp1251�, �koi8r�,�)

6)      ��������� ������ BigDump � �������.

7)      � ����������� �������� ������ ������ Start.

8)      ��������� ��������� �������� �� ������.

9)      ������!
������� ���������� ��� ������������� - ������� 2:

    ��������� ������ ����� �� �������. ����� ������� ��������� � ������, �� ������������� ������� ��������� ����� � ��������� ���� ���� ������.
    ����� �������� ���������� ��������������� ���� ������ ������ ����� ���� ������������ (���������� $db_name), ��� ������������ (���������� $db_username) � ������ (���������� $db_password).
    �������� ���� ������. ��������: site35.ru/bigdump.php
    �������� ���� �����. �� ����� ���� ��� ��������� ������ (sql/csv), ��� � ������� - gz.
    ����� ����� �������� ������� ������ �������� �� ������ "Start import".
    ����� ������� ����� ����� ���������� ��� ���������� �������.

�������� ������� �������������:

    �� �������� ��������� ��������� ��������� ��� ����� ����� � ������� bigdump.php, �� �� �������� ���������� $db_connection_charset. �� ��������� ��� ������. ���� � ��� ���� � ��������� UTF-8, �� ���������� ���������� $db_connection_charset = �utf8?;
    �� �������� ���������� ����� �� ����� � ������� ����� ���� �� chmod 777
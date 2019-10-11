# Oregon_NR
/////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
// This Arduino code is for receive and transmit data using Oregon Scientific RF protocol version 2.1 and 3.0. 
//
// Last updated: 11 �ctober 2019
//
// The folowed sensors data format are supported.
//
// Receive and transmit:
// THGN132N (THGR122N, THGN123N),
// RTGN318,
// THGR810.

// Receive only:
// THN132N,
// WGR800,	
// UVN800.
//
// Aslo supported self-developed sensors. Please contact author for additional infromation.
/////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
//
// ������ ���������� ������� ������������� ��� ������ � �������� ������ � ������� ������������� ��������� Oregon Scientific v2.1 � v3.0
//
// ��������� ���������� 11 ������� 2019
//
// �������������� ������ ��������� ��������
//
// ���� � ��������:
// THGN132N (THGR122N, THGN123N),
// RTGN318,
// THGR810.

// ������ ����:
// THN132N,
// WGR800,	
// UVN800.
//
// ����� �������������� ������� ����������� ���������� (�� �������������� ������������ ���������� � ������)
/////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
//
// ��� �������� ������������� �� ������������ �������� THGN132N, THN132N � WGR800.
//
// ��� ����������� ��������������� �� �������� �������� BAR206, BAR208 ��������� ������� THGN132N
// ��� ��������� ����� �������� �������� ������� ���������� ��������� ��������� ������� ��� �������� ������:
// ��������� 2-98%
// ����������� -50...+70�
// ��� �������� ����������������� �������� � ������� "��������� ���" ����� ������, ��� ��������� ����� �������� ��� ��������� ����� �������� �������� 
// ������ ���������� �� ����������� �� ����� ��� �� +-1���. �������� ��� THGN132:
// ����� 1 - 39 (38 - 40) c 
// ����� 2 - 41 (40 - 42) c
// ����� 3 - 43 (42 - 44) c
//
// ���� ������ ����� � ���������� CRC � ����������� ������, �� �������� ����������� � ��������� ������������, �������� +3.0� �������� �� ��� 0300, � A200
// �� ������ ����� ���� ������������ �� ����� ID ��� �� ������ �������� ��������.
// ���������� �������� �������� � ��� ������������ ��������� ������ ������ � ID �������. ���� ������ ���� �� ����� �� ������
//
// �������� �������� � ������� RTGN318 � THGR810 �� ����� �� ��������������. ������� �������� �������� � ������ ���� �������� �������� ��������
// �� ��������� �������
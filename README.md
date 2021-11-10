#!/bin/bash


if ( -z $ROS_MASTER_URI );then
        echo "[Check]environment bariable ...Wrong"
else
        echo "[Check]environment bariable ...Pass"
fi




IPADDRESS=$ROS_MASTER_URI
regex="http://[0-9][0-9][0-9].[0-9][0-9][0-9].[0-9].[0-9][0-9][0-9]:[0-9][0-9][0-9][0-9][0-9]"

if ( IPADDRESS=regax )
then
       echo "[Check] address validation...   Wrong"
else
       echo "[Check] address validation...   Pass"
fi




if ( ping -q http://192.168.0.100:11311="http://192.168.0.100:11311" )
then
        echo "[Check] ping address...         Pass"

else
        echo "[Check] ping address...         Wrong"

fi


